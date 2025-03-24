[![MasterHead](https://raw.githubusercontent.com/thekurup/thekurup/main/github-header.gif)](https://arjunkurup.com)
<h1 align="center">Hi 👋, I'm Arjun Kurup</h1>
<h3 align="center">Flutter Engineer | Architecture Specialist | Technical Mentor</h3>

<p align="center">
  <a href="https://twitter.com/arjunkurup_" target="blank">
    <img src="https://img.shields.io/badge/Twitter-Follow_@arjunkurup_-blue?style=flat&logo=twitter" alt="Twitter Follow"/>
  </a>
  <a href="https://linkedin.com/in/arjun-kurup/" target="blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect_Now-0077B5?style=flat&logo=linkedin" alt="LinkedIn"/>
  </a>
  <a href="https://bento.me/arjunkurup">
    <img src="https://img.shields.io/badge/Portfolio-View_Projects-FF4088?style=flat&logo=react" alt="Portfolio"/>
  </a>
</p>

---

### 💼 Technical Leadership Proposition
**I solve critical engineering challenges for scaling teams:**  
✅ **Zero-Crash Releases** → 85%+ test coverage with CI/CD guardrails  
✅ **Future-Proof Architecture** → Production-grade Riverpod implementations  
✅ **Developer Velocity** → Cut release cycles from weeks to days  
✅ **Team Enablement** → Authored 15+ technical guides with 50k+ reads  

---

### ⚡ Technical Arsenal
<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.19-blue?logo=flutter" />
  <img src="https://img.shields.io/badge/Riverpod-2.3-FF6B6B?logo=dart" />
  <img src="https://img.shields.io/badge/Hive-2.2.3-FFCA28" />
  <img src="https://img.shields.io/badge/CI/CD-Auto_Deploy-2088FF?logo=githubactions" />
  <img src="https://img.shields.io/badge/Testing-85%25_Coverage-brightgreen" />
  <img src="https://img.shields.io/badge/Architecture-Clean_TDD-6DB33F" />
</p>

---

### 🚀 Production-Grade Impact
| Project | Technical Leadership | Business Impact |
|---------|----------------------|-----------------|
| **[E-Commerce App](link)** | • Migrated to Riverpod state management<br>• Hive DB performance optimization<br>• GitHub Actions CI/CD pipeline | • 30% faster cart operations<br>• 85% test coverage |
| **[EdTech Platform (WIP)](link)** | • Clean Architecture implementation<br>• Firebase Auth + Firestore integration<br>• Modular dependency injection | • Scalable to 10k+ users<br>• TDD implementation guide |
| **[Flutter DevOps Kit](link)** | • Automated testing workflow<br>• Fastlane multi-environment support | • 50+ dev adoption<br>• 40% faster deployments |

---

### 💡 Hiring Manager Solutions
**I specialize in:**  

| Problem | My Solution | Proof |  
|---------|-------------|-------|  
| **"Production crashes cost us $10k/month"** | TDD + Crashlytics integration | [Test Report](link) |  
| **"2-week release cycles"** | CI/CD pipeline implementation | [Workflow File](link) |  
| **"Unmaintainable codebase"** | Clean Architecture migration | [Case Study](link) |  
| **"Junior team blockers"** | Modular code examples + docs | [Guide](link) |  

📩 **Challenge:** Send your toughest technical debt → I'll propose a solution within 48h  

---

### 📊 Engineering Velocity
<p align="center">
  <img width="45%" src="https://github-readme-stats.vercel.app/api?username=thekurup&show_icons=true&theme=radical&hide_border=true&count_private=true" alt="Contribution Stats"/>
  <img width="45%" src="https://github-readme-streak-stats.herokuapp.com/?user=thekurup&theme=dark&hide_border=true" alt="Commit Streak"/>
</p>

```dart
// Clean Architecture Implementation
@Riverpod(keepAlive: true)
class AuthController extends _$AuthController {
  @override
  FutureOr<User> build() async {
    return ref.watch(authRepositoryProvider).getCurrentUser();
  }
  
  Future<void> signIn(String email, String password) async {
    state = const AsyncValue.loading();
    state = await AsyncValue.guard(() => 
      ref.read(authRepositoryProvider).signIn(email, password));
  }
}
