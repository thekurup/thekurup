[![MasterHead](https://raw.githubusercontent.com/thekurup/thekurup/main/github-header.gif)](https://arjunkurup.com)
<h1 align="center">Hi 👋, I'm Arjun Kurup</h1>
<h3 align="center">Flutter Engineer | Technical Architect | Continuous Learner</h3>




<p align="center">
  <a href="https://twitter.com/arjunkurup_" target="blank">
    <img src="https://img.shields.io/badge/Twitter-Get_Flutter_Tips-blue?style=flat&logo=twitter" alt="Twitter"/>
  </a>
  <a href="https://linkedin.com/in/arjun-kurup/" target="blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect_for_Opportunities-0077B5?style=flat&logo=linkedin" alt="LinkedIn"/>
  </a>
  <a href="https://bento.me/arjunkurup">
    <img src="https://img.shields.io/badge/Portfolio-See_My_Journey-FF4088?style=flat&logo=react" alt="Portfolio"/>
  </a>
</p>


---

### 🚀 Value Proposition for Tech Teams
**I Have done:**  
✅ **Production Deployment** → Published EdTech app with 85% coverage  
✅ **CI/CD Automation** → Automated testing+deployment pipeline  
✅ **Modern Architecture** → Riverpod + Clean Architecture implementation  
✅ **Team Enablement** → Created 3 onboarding guides  
✅ **Knowledge Sharing** → 15+ technical articles with proven adoption  

---

### ⚡ Verified Technical Stack
<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.19.3-blue?logo=flutter" />
  <img src="https://img.shields.io/badge/Dart-3.3.0-0175C2?logo=dart" />
  <img src="https://img.shields.io/badge/Riverpod-2.3.6-FF6B6B" />
  <img src="https://img.shields.io/badge/CI/CD-GitHub_Actions-2088FF?logo=github" />
  <img src="https://img.shields.io/badge/Testing-87%25_Coverage-brightgreen" />
</p>

### 💡 Hiring Manager Solutions
**I specialize in:**  

| Problem | My Solution | Proof |  
|---------|-------------|-------|  
| **"Frequent app crashes"** | TDD with 85% coverage + Crashlytics | [Test Report](link) |  
| **"2-week release cycles"** | CI/CD pipeline implementation | [Workflow File](link) |  
| **"Unmaintainable codebase"** | Clean Architecture migration | [Case Study](link) |  
| **"New devs struggle"** | Modular code examples + docs | [Guide](link) | 

---

### 🏗️ Project Impact Showcase
| Project | Technical Milestones | Measurable Outcomes |
|---------|-----------------------|---------------------|
| **[E-Commerce App](link)** | • Hive DB optimization<br>• TDD implementation<br> | • 85% test coverage<br>• 30% faster local ops |
| **[EdTech Platform (WIP)](link)** | • Riverpod state management <br>• Firebase Auth integration<br>• CI/CD Pipeline | • Scalability blueprint<br>• TDD implementation guide |
| **[Flutter Starter Kit](link)** | • GitHub Actions template<br>• Modular architecture | • 20+ GitHub stars<br>  |

---
### 📊 Engineering Velocity
<p align="center">
  <img width="45%" src="https://github-readme-streak-stats.herokuapp.com/?user=thekurup&theme=dark&hide_border=true" alt="Commit Streak">
  <img width="45%" src="https://github-readme-stats.vercel.app/api?username=thekurup&show_icons=true&theme=radical&hide_border=true&count_private=true" alt="Contribution Stats"/>
  <img width="45%" src="https://github-readme-streak-stats.herokuapp.com/?user=thekurup&theme=dark&hide_border=true" alt="Commit Streak">
</p>

### 🔍 Technical Depth Preview
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
