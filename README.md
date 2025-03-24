[![MasterHead](https://raw.githubusercontent.com/thekurup/thekurup/main/github-header.gif)](https://arjunkurup.com)
<h1 align="center">Hi 👋, I'm Arjun Kurup</h1>
<h3 align="center">Flutter Engineer | Clean Code Advocate | Technical Writer</h3>

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

### 💼 8 LPA-Ready Value Proposition
**I excel at:**  
✅ **Production-Grade Code** → 85%+ test coverage in personal projects  
✅ **Modern Architecture** → Migrated from setState to Riverpod in active project  
✅ **CI/CD Implementation** → Automated testing & deployment pipelines  
✅ **Knowledge Sharing** → 15+ technical articles with 50k+ reads  

---

### ⚡ Technical Arsenal
<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.19-blue?logo=flutter" />
  <img src="https://img.shields.io/badge/Riverpod-2.3-FF6B6B?logo=dart" />
  <img src="https://img.shields.io/badge/Hive-Local_DB-FFCA28" />
  <img src="https://img.shields.io/badge/CI/CD-Auto_Deploy-2088FF?logo=githubactions" />
  <img src="https://img.shields.io/badge/Testing-85%25_Coverage-brightgreen" />
</p>

---

### 🏗️ Production-Grade Projects
| Project | Tech Stack | Key Achievements |
|---------|------------|------------------|
| **[E-Commerce App](link)** | Flutter • Hive • REST API | • Optimized local cache<br>• CI/CD pipeline implementation<br>• State management migration analysis |
| **[EdTech App (WIP)](link)** | Flutter • Riverpod • Firebase | • Clean Architecture setup<br>• Modular navigation system<br>• TDD implementation guide |
| **[Flutter CI/CD Template](link)** | GitHub Actions • Fastlane | • Auto APK builds on PR merge<br>• Used by 30+ developers |
| **[Open Source Contributions](link)** | Flutter Community | • Authored testing guide with 500+ claps<br>• Documented Riverpod best practices |

---

### 📊 Code Warfare Stats
<p align="center">
  <img width="45%" src="https://github-readme-stats.vercel.app/api?username=thekurup&show_icons=true&theme=radical&hide_border=true&count_private=true" />
  <img width="45%" src="https://github-readme-streak-stats.herokuapp.com/?user=thekurup&theme=dark&hide_border=true" />
</p>

```dart
// Current Architecture Exploration
class EdTechApp extends ConsumerWidget {
  const EdTechApp({super.key});

  @override
  Widget build(BuildContext context, WidgetRef ref) {
    final router = ref.watch(routerProvider);
    return MaterialApp.router(
      routerConfig: router,
      theme: AppTheme.light(),
      debugShowCheckedModeBanner: false,
    );
  }
}
