# 📱 Flutter Quiz App

An interactive quiz app built using **Flutter**, where users can test their knowledge through multiple-choice questions and view a detailed summary of their answers. Designed with clean UI and responsive layout principles.

---

## ✨ Features

- Interactive multiple-choice questions
- Displays correct vs user-selected answers
- Result summary screen
- Option to restart the quiz
- Built using modern **Flutter widget architecture**

---

## 🧠 Concepts Covered

- **Stateless vs Stateful Widgets**
- **ListView, Column, Row layouts**
- **Data Passing Between Screens**
- **Custom Widgets**
- **Safe casting & null safety in Dart**
- **Flutter theming and styling**
- **Local state management**
- **Dynamic UI rendering based on user input**

---

## 🛠️ Getting Started

### ✅ Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) installed
- Android Studio OR Visual Studio Code with Flutter/Dart plugins
- Emulator or a real device configured

---

## 🚀 Setup Instructions

### 1. Clone the Repository

### 2. Install Packages
flutter pub get

### 3. Launch the App
flutter run

Ensure that an emulator is running or a device is connected.

📂 Project Structure
lib/
├── data/
│   └── questions.dart         # List of quiz questions
├── models/
│   └── quiz_question.dart     # Model class for quiz questions
├── screens/
│   ├── start_screen.dart      # Start button and intro
│   ├── question_screen.dart   # Main quiz logic
│   └── result_screen.dart     # Summary + score display
│── answer_button.dart     # Custom Answer button
└── questions_summary.dart # Summary rows widget
└── main.dart                  # App entry and navigation

🧪 Example Quiz Questions
What are the main building blocks of Flutter UIs?

How are Flutter UIs built?

What's the purpose of a StatefulWidget?

What happens if you change data in a StatelessWidget?

🖼️ Screenshots
Quiz Screen	Result Summary
image.png 

🔄 Restart Quiz Logic
We use setState() and a screen-swapping mechanism using StatefulWidget in main.dart to go back to the start screen when the "Restart Quiz" button is pressed.

🧩 How It Works
1.User taps "Start Quiz"

2. Question screen shows questions one-by-one

3. Each answer is saved to a List<String> called chosenAnswers

4. When quiz ends, result screen uses:
summaryData.where((data) => data['user_answer'] == data['correct_answer'])

To calculate score and display question-wise summary.

👨‍💻 Contributing
Feel free to fork the project and send a PR! Open to improvements and new features like:
Timer for each question
Category-based questions
Animated transitions

📜 License
This project is open source under the MIT License.

🙌 Acknowledgements
Inspired by Flutter’s official documentation and course content by Maximilian Schwarzmüller (Academind).

📬 Contact
Made with ❤️ by Ashmit
For suggestions: ashmitmala002@gmail.com
