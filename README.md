# 🎓 Quiz Master - Flutter Quiz Application

A professional, feature-rich quiz application built with Flutter that provides an engaging learning experience with multiple categories, timed questions, and comprehensive result analysis.



## 📱 Screenshots

<img width="315" height="700" alt="Screenshot_1764815677" src="https://github.com/user-attachments/assets/4caaa3a0-833c-436f-9722-b31ce7624d68" />

<img width="315" height="700" alt="Screenshot_1764815754" src="https://github.com/user-attachments/assets/71bb24c8-094e-4ad7-920c-49eeaf6fe6d7" />
<img width="315" height="700" alt="Screenshot_1764815747" src="https://github.com/user-attachments/assets/4acf38ec-4479-4a81-88c5-4b2cfd5366fb" />
<img width="315" height="700" alt="Screenshot_1764815721" src="https://github.com/user-attachments/assets/64abcdfc-3d82-49db-ac9d-e3f361992dbb" />
<img width="315" height="700" alt="Screenshot_1764815708" src="https://github.com/user-attachments/assets/c8a4091e-a836-488e-b842-b649575502ba" />
<img width="315" height="700" alt="Screenshot_1764815693" src="https://github.com/user-attachments/assets/363d26d2-17be-49cb-8c7a-74cb6456d4d3" />





## ✨ Features

### 🎯 Core Features
- **Multiple Quiz Categories**: General Knowledge, Technology, and Science
- **15 Questions Per Category**: Comprehensive question sets for thorough testing
- **Timed Questions**: 15-second countdown timer for each question
- **Answer Shuffling**: Options are randomized on every quiz attempt to prevent memorization
- **Progress Tracking**: Visual progress bar showing quiz completion
- **Detailed Results**: Comprehensive performance analysis with statistics

### 🎨 Design & UI/UX
- **Material 3 Design**: Modern, clean interface following Google's latest design guidelines
- **Light & Dark Theme**: Automatic theme switching based on system preferences
- **Smooth Animations**: Polished transitions and micro-interactions
- **Color-Coded Feedback**: Visual indicators for correct/incorrect/skipped answers
- **Responsive Layout**: Optimized for various screen sizes

### 📊 Result Analysis
- **Performance Summary**: Score percentage with motivational messages
- **Statistics Dashboard**: Breakdown of correct, wrong, and skipped answers
- **Question Review**: Detailed review of each question with:
  - User's selected answer
  - Correct answer
  - Explanations for better understanding
- **Performance Icons**: Visual feedback based on score (Trophy, Thumbs Up, etc.)

### ⚡ Additional Features
- **Exit Confirmation**: Prevents accidental quiz exits
- **Auto-Advance**: Automatic progression to next question
- **Timer Warnings**: Color-coded timer (Green → Orange → Red)
- **Category Icons**: Visual representation for each quiz category
- **Explanation Cards**: Educational content after each answer

## 🚀 Getting Started

### Prerequisites

- Flutter SDK (3.0.0 or higher)
- Dart SDK (3.0.0 or higher)
- Android Studio / VS Code with Flutter extensions
- An Android/iOS emulator or physical device

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/AnishTiwari077/Flutter-quiz-master.git
   cd quiz-master
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

### Build for Production

**Android APK:**
```bash
flutter build apk --release
```

**iOS:**
```bash
flutter build ios --release
```

## 📁 Project Structure

```
lib/
├── main.dart                      # App entry point
├── theme/
│   └── app_theme.dart            # Theme configuration & colors
├── models/
│   └── question_model.dart       # Question data model with shuffle logic
├── data/
│   └── question_data.dart        # Quiz questions database
├── screens/
│   ├── home_screen.dart          # Category selection screen
│   ├── quiz_screen.dart          # Quiz gameplay screen
│   └── result_screen.dart        # Results & review screen
└── widgets/
    └── option_card.dart          # Reusable option button widget
```

## 🎮 How to Use

1. **Launch the app** - You'll see the home screen with available categories
2. **Select a category** - Choose from General Knowledge, Technology, or Science
3. **Answer questions** - You have 15 seconds per question
4. **Review results** - See your score, statistics, and detailed question review
5. **Retry or go home** - Choose to retry the quiz or select a new category

## 🎨 Customization

### Adding New Questions

Edit `lib/data/question_data.dart`:

```dart
'Your Category': [
  Question(
    question: 'Your question text?',
    options: ['Option A', 'Option B', 'Option C', 'Option D'],
    correctIndex: 0, // Index of the correct answer (0-3)
    explanation: 'Explanation of the correct answer',
  ),
  // Add more questions...
],
```

### Changing Colors

Edit `lib/theme/app_theme.dart`:

```dart
static const Color primaryColor = Color(0xFF2196F3);
static const Color secondaryColor = Color(0xFF03DAC6);
static const Color errorColor = Color(0xFFEF5350);
static const Color successColor = Color(0xFF66BB6A);
```

### Adjusting Timer Duration

Edit `lib/screens/quiz_screen.dart`:

```dart
void startTimer() {
  timeLeft = 15; // Change to your desired duration in seconds
  // ...
}
```

## 🏗️ Architecture

### Design Patterns
- **Separation of Concerns**: Clear separation between UI, data, and business logic
- **Reusable Widgets**: Modular components for maintainability
- **State Management**: StatefulWidget with proper lifecycle management

### Key Classes

**Question Model**
- Stores question data
- Handles answer shuffling logic
- Tracks correct answer index

**Quiz Screen**
- Manages quiz state and timer
- Handles user interactions
- Controls question flow

**Result Screen**
- Displays performance metrics
- Shows detailed question review
- Compares shuffled vs original answers

## 📊 Features Breakdown

### Answer Shuffling Algorithm
```dart
Question shuffleOptions() {
  // Creates indexed list of options
  // Shuffles while tracking correct answer position
  // Returns new Question with shuffled options
}
```

### Performance Grading
- **80-100%**: Excellent! 🎉 (Green)
- **60-79%**: Good Job! 👍 (Blue)
- **40-59%**: Keep Practicing! 💪 (Orange)
- **0-39%**: Don't Give Up! 📚 (Red)

## 🔧 Technical Stack

- **Framework**: Flutter 3.x
- **Language**: Dart 3.x
- **Design**: Material Design 3
- **State Management**: StatefulWidget
- **Navigation**: Flutter Navigator 2.0

## 📝 Code Quality

- ✅ Null safety enabled
- ✅ Clean code architecture
- ✅ Comprehensive documentation
- ✅ Reusable components
- ✅ Proper error handling
- ✅ Memory leak prevention (timer disposal)

## 🐛 Known Issues

Currently no known issues. If you find any bugs, please open an issue.


### Contribution Ideas
- Add more quiz categories
- Implement difficulty levels
- Add sound effects
- Create leaderboard system
- Add social sharing
- Implement local storage for progress tracking
- Add animations and lottie files
- Multi-language support



## 👨‍💻 Author

**Your Name**
- GitHub: [@AnishTiwari5077](https://github.com/AnishTiwari5077)


## 🙏 Acknowledgments

- Flutter team for the amazing framework
- Material Design team for design guidelines
- All contributors who help improve this project






<div align="center">

**Made with ❤️ using Flutter**

If you like this project, please give it a ⭐!

</div>
