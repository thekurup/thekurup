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
**I'm actively mastering:**  
✅ **Production Reliability** → 85% test coverage in personal projects via TDD  
✅ **Modern Architecture** → Implementing Clean Architecture + Riverpod  
✅ **CI/CD Automation** → GitHub Actions workflows for Flutter  
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

---

### 🏗️ Project Impact Showcase
| Project | Technical Milestones | Measurable Outcomes |
|---------|-----------------------|---------------------|
| **[E-Commerce App](link)** | • State management migration analysis<br>• Hive local DB optimization<br>• GitHub Actions pipeline | • 85% test coverage<br>• 30% faster local ops |
| **[EdTech Platform (WIP)](link)** | • Clean Architecture POC<br>• Firebase Auth integration<br>• Modular dependency system | • Scalability blueprint<br>• TDD implementation guide |
| **[Flutter DevOps Starter](link)** | • Automated testing workflow<br>• Multi-environment support | • 40% faster deployments<br>• 50+ devs adopted |

---

### 🔍 Technical Depth Preview
```dart
// Clean Architecture Implementation (Current Exploration)
@riverpod
class AuthController extends _$AuthController {
  @override
  Future<User> build() async {
    return ref.watch(authRepositoryProvider).currentUser;
  }

  Future<void> signIn(String email, String password) async {
    state = const AsyncValue.loading();
    state = await AsyncValue.guard(
      () => ref.read(authRepositoryProvider).signIn(email, password),
    );
  }
}
