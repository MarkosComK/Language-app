# AI Language Learning App

A modern language learning application built with Flutter, featuring AI-powered conversations and a freemium business model.

## Features

### Free Tier
- AI-powered conversation practice with daily limits
- Basic progress tracking
- Community features
- Ad-supported content
- Core language lessons

### Premium Tier
- Unlimited AI conversations
- Advanced grammar correction
- Real-time pronunciation analysis
- Downloadable learning materials
- Ad-free experience
- Personalized learning paths
- Detailed progress analytics
- Support for multiple languages

## Technical Stack

### Frontend
- Flutter for cross-platform development
- Provider for state management
- Material Design 3 components
- Local storage for offline functionality

### Backend
- Firebase Authentication
- Cloud Firestore
- Firebase Cloud Functions
- Firebase Storage
- Stripe payment processing

## Project Setup

### Prerequisites
- Flutter SDK (Latest stable version)
- Firebase CLI
- Node.js (for Cloud Functions)
- Android Studio / Xcode
- A Firebase project
- Stripe account

### Getting Started

1. Clone the repository
```bash
git clone https://github.com/yourusername/language-learning-app.git
cd language-learning-app
```

2. Install dependencies
```bash
flutter pub get
```

3. Configure Firebase
```bash
firebase init
```

4. Set up your Firebase configuration files
- Add `google-services.json` to `android/app/`
- Add `GoogleService-Info.plist` to `ios/Runner/`

5. Configure environment variables
```bash
cp .env.example .env
```
Edit `.env` with your API keys and configuration values.

## Project Structure
```
lib/
├── main.dart
├── app/
│   ├── app.dart
│   └── router.dart
├── features/
│   ├── auth/
│   ├── chat/
│   ├── lessons/
│   ├── premium/
│   └── profile/
├── core/
│   ├── constants/
│   ├── services/
│   └── widgets/
└── shared/
    ├── models/
    ├── utilities/
    └── widgets/
```

## Development Guidelines

### Code Style
- Follow Flutter's style guide
- Use meaningful variable and function names
- Document complex functionality
- Write unit tests for business logic

### Git Workflow
1. Create feature branches from `develop`
2. Use conventional commits
3. Submit PRs for review
4. Merge to `develop` after approval
5. Release from `develop` to `main`

### Testing
```bash
# Run unit tests
flutter test

# Run integration tests
flutter drive --target=test_driver/app.dart
```

## Monetization Implementation

### Stripe Integration
1. Set up Stripe webhook endpoints in Firebase Functions
2. Implement subscription management
3. Handle payment lifecycle events
4. Set up recurring billing

### Premium Features Control
- Use Firebase Remote Config for feature flags
- Implement subscription status checks
- Handle subscription state changes
- Manage entitlements

## Deployment

### Android
1. Update `version` in `pubspec.yaml`
2. Build release APK/Bundle
```bash
flutter build appbundle --release
```

### iOS
1. Update version and build number
2. Build release IPA
```bash
flutter build ips --release
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## Support
For support, email support@yourdomain.com or join our Slack channel.
