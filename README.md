# 🩺 Medical AI Assistant Using Gemini

![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)
![Gemini API](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=google&logoColor=white)
![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)

## 📖 Description

**Medical AI Assistant** is a cross-platform mobile application built with **Flutter** that leverages the power of **Google's Gemini API** (specifically the `gemini-2.0-flash` model). This app acts as an intelligent virtual health companion, capable of analyzing symptoms and answering medical queries in a clean, conversational interface.

The app utilizes the **Flutter AI Toolkit** to provide a polished chat UI (LlmChatView) with pre-defined suggestions and strictly prompted system instructions to ensure the AI remains focused solely on medical and health-related topics.

## ✨ Key Features

*   **🤖 Specialized Medical AI:** Custom system instructions ensure the AI only answers health-related questions and politely declines unrelated queries.
*   **💬 Modern Chat Interface:** Built using `flutter_ai_toolkit` for a seamless chat experience with typing indicators and bubble styling.
*   **⚡ Gemini 2.0 Flash:** Powered by Google's latest fast-inference model for instant responses.
*   **💡 Smart Suggestions:** Includes quick-start prompts like "What should I eat to boost my immunity?"
*   **🎨 Clean Architecture:** Simple, single-screen implementation for ease of use and learning.

## 🚀 Getting Started

Follow these steps to run the project locally.

### Prerequisites
*   [Flutter SDK](https://flutter.dev/docs/get-started/install) installed.
*   A [Google Gemini API Key](https://aistudio.google.com/app/apikey).

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/your-username/medical-ai-assistant.git
    cd medical-ai-assistant
    ```

2.  **Install dependencies**
    ```bash
    flutter pub get
    ```

3.  **🔑 Configure API Key**
    To run the app, you must manually insert your Gemini API key into the source code:
    
    1. Open the file `lib/chat.dart` (or `lib/screens/chat.dart` depending on your folder structure).
    2. Locate the `_MedicalChatScreenState` class.
    3. Find the variable `apiKey` and paste your key inside the quotes:
    
    ```dart
    // Inside lib/chat.dart
    class _MedicalChatScreenState extends State<MedicalChatScreen> {
      // REPLACE THIS LINE WITH YOUR KEY
      String apiKey = "YOUR_ACTUAL_GEMINI_API_KEY_HERE"; 
      
      @override
      void initState() {
        super.initState();
      }
      // ...
    ```

4.  **Run the App**
    ```bash
    flutter run
    ```

## ⚠️ Important Security Note

**Do not commit your API Key to GitHub!** 
Since the API key is hardcoded in `chat.dart`, be careful not to push your actual key to a public repository. If you plan to share this code, remove your key and replace it with an empty string `""` before committing.

## ⚠️ Medical Disclaimer

**Please Note:** This application uses Artificial Intelligence to provide information and is intended for educational and informational purposes only. It is **not** a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or qualified health provider with any questions you may have regarding a medical condition.

## 🤝 Contribution

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## ☕ Donate

If you found this project helpful or want to support my work, feel free to buy me a coffee!

<a href="https://www.buymeacoffee.com/gonzotrickster9899" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

---

*Built with ❤️ using Flutter, Flutter AI Toolkit, and Google Gemini.*