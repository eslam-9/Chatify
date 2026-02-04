# Chatify 💬

A modern real-time chat application built with Flutter and Supabase, featuring user authentication, real-time messaging, and a clean, intuitive interface.

## ✨ Features

- **User Authentication**
  - Sign up with email and password
  - Secure sign-in functionality
  - User profile management

- **Real-time Chat**
  - Instant messaging powered by Supabase
  - Real-time message updates
  - User information display

- **Modern UI/UX**
  - Clean and intuitive interface
  - Custom theming with consistent color scheme
  - Responsive design
  - Image picker integration for profile pictures

## 🛠️ Tech Stack

- **Framework**: Flutter 3.5.0
- **Backend**: Supabase (Authentication & Real-time Database)
- **State Management**: Provider
- **Navigation**: GoRouter
- **Additional Packages**:
  - `image_picker` - For selecting profile images
  - `path` - Path manipulation utilities

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Flutter SDK (3.5.0 or higher)
- Dart SDK (3.5.0 or higher)
- Android Studio / VS Code with Flutter extensions
- A Supabase account and project

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/eslam-9/chatify.git
cd chatify
```

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Supabase Configuration

This project uses Supabase for backend services. You'll need to:

1. Create a project on [Supabase](https://supabase.com)
2. Set up authentication (Email/Password provider)
3. Create necessary database tables for users and messages
4. Update the Supabase credentials in `lib/main.dart`:

```dart
await Supabase.initialize(
  url: "YOUR_SUPABASE_URL",
  anonKey: "YOUR_SUPABASE_ANON_KEY",
);
```

### 4. Run the Application

```bash
flutter run
```

## 📁 Project Structure

```
lib/
├── logic/              # Business logic and state management
│   ├── authorization.dart
│   ├── chat_logic.dart
│   ├── user_provider.dart
│   └── nwe.dart
├── screens/            # UI screens
│   ├── chat/          # Chat interface
│   │   ├── chat.dart
│   │   └── massege_field.dart
│   ├── information/   # User information screen
│   │   └── informations.dart
│   ├── sign_in/       # Sign-in screen
│   │   └── signin.dart
│   └── signup/        # Sign-up screen
│       ├── signup.dart
│       └── textfieldmake.dart
├── theaming/          # Theme and styling
│   └── color.dart
└── main.dart          # Application entry point
```

## 🎨 Theming

The app uses a custom color scheme defined in `lib/theaming/color.dart` with:
- Primary color: Main blue
- Background color: Custom background

## 🔐 Security Note

**Important**: The current Supabase credentials in the code are exposed. For production use:
1. Move credentials to environment variables
2. Use `.env` files (not committed to version control)
3. Implement proper security rules in Supabase

## 📱 Supported Platforms

- ✅ Android
- ✅ iOS
- ✅ Web
- ✅ Windows

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request




## 🙏 Acknowledgments

- Flutter team for the amazing framework
- Supabase for the backend infrastructure
- All contributors who help improve this project

