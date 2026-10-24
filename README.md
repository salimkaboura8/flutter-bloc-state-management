<div align="center">

# 🧩 Flutter BLoC State Management

**A true/false quiz app showing how to manage state with the BLoC pattern**

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![BLoC](https://img.shields.io/badge/BLoC-Pattern-13B9FD?style=for-the-badge)

[📂 Source](lib) · [🧠 Business Logic](lib/business_logic) · [🎨 UI](lib/presentation)

</div>

---

## 📖 Overview

A French geography and history quiz built with **Flutter**. Each question has a **True** (*Vrai*) or **False** (*Faux*) answer, and the score is kept by a `QuizBloc`. The project keeps the UI apart from the business logic, which makes the BLoC pattern easy to follow.

## 🔄 How It Works

| Step | What happens |
|:---:|---|
| 1️⃣ | The app starts with an initial `QuizState` (questions, answers, index, score) |
| 2️⃣ | Tapping **Vrai** or **Faux** dispatches a `NextQuestion` event to the BLoC |
| 3️⃣ | `QuizBloc` checks the answer, updates the score and emits a new state |
| 4️⃣ | The UI rebuilds with the next question, or shows the final score at the end |

## ✨ Highlights

| 🧠 State | 🎨 UI | 🧱 Architecture |
|---|---|---|
| `flutter_bloc` events and states<br>Immutable `QuizState`<br>Score tracking | Image and question card<br>True / False buttons<br>Final score screen | `data` / `business_logic` / `presentation` layers<br>Single source of truth |

## 🚀 Quick Start

```bash
git clone https://github.com/salimkaboura8/flutter-bloc-state-management.git
cd flutter-bloc-state-management

flutter pub get
flutter run
```

---

<div align="center">
Made with ❤️ by <a href="https://github.com/salimkaboura8">Salim Kaboura</a>
</div>
