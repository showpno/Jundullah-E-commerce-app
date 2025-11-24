# 🛍️ Jundullah Lifestyle - E-Commerce Mobile App

A modern, fully-featured e-commerce mobile application built with Flutter, providing a seamless shopping experience with a beautiful UI and robust functionality.

## ✨ Features

- 🏠 **Home Screen** - Browse featured products and categories
- 🔐 **Authentication** - Secure user registration and login
- 🛒 **Shopping Cart** - Add, remove, and manage products
- ❤️ **Favorites** - Save your favorite products
- 📦 **Order Management** - Track orders from placement to delivery
- 👤 **User Profile** - Manage account and address information
- 🔍 **Search & Filter** - Find products quickly
- 💳 **Multiple Payment Options** - COD and Prepaid support
- 📱 **Responsive Design** - Works on all Android devices

## 🚀 Getting Started

### Prerequisites

- Flutter SDK (>=3.4.3)
- Dart SDK
- Android Studio / VS Code
- Android Emulator or Physical Device

### Installation

1. Clone the repository:
```bash
git clone https://github.com/showpno/Jundullah-E-commerce-app.git
cd Jundullah-E-commerce-app/client_side/nexara_cart/client_side
```

2. Install dependencies:
```bash
flutter pub get
```

3. Configure server URL:
   - Open `lib/utility/server_config.dart`
   - Set `manualPhysicalDeviceIP` to your local IP address for physical device testing
   - For emulator, it will use `10.0.2.2` automatically
   - Use `get_local_ip.ps1` script to find your local IP address

4. Run the app:
```bash
flutter run
```

Or use the provided scripts:
- `run.ps1` - Interactive device selection (PowerShell)
- `run.bat` - Interactive device selection (CMD)

## 🔧 Configuration

### Server Configuration

The app automatically detects the device type and configures the server URL:

- **Android Emulator**: Uses `10.0.2.2` (maps to host machine's localhost)
- **Physical Device**: Requires manual IP configuration

To configure for physical device:
1. Run `.\get_local_ip.ps1` to get your local IP
2. Update `lib/utility/server_config.dart`:
   ```dart
   static const String? manualPhysicalDeviceIP = '192.168.1.100'; // Your IP
   ```
3. Ensure your device and computer are on the same Wi-Fi network

### Environment Setup

- Server Port: Default is `5000` (configurable in `server_config.dart`)
- API Endpoints: Configured in `lib/services/http_services.dart`
- Constants: App-wide constants in `lib/utility/constants.dart`

## 📁 Project Structure

```
lib/
├── core/
│   └── data/          # Data providers
├── models/            # Data models
├── screen/            # UI screens
│   ├── auth_screen/   # Login & Registration
│   ├── product_*/     # Product related screens
│   └── ...
├── services/          # API services
├── utility/           # Utilities & helpers
│   ├── constants.dart
│   ├── server_config.dart
│   └── ...
└── widget/            # Reusable widgets
```

## 🛠️ Technologies Used

- **Flutter** - UI Framework
- **GetX** - State management & routing
- **Provider** - State management
- **Get Storage** - Local storage
- **HTTP Services** - API communication
- **Device Info Plus** - Device detection

## 📱 Screenshots

*(Add screenshots of your app here)*

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is private and proprietary.

## 👨‍💻 Author

**Showpno**
- GitHub: [@showpno](https://github.com/showpno)

## 🙏 Acknowledgments

- Flutter community
- All contributors and supporters

---

Made with ❤️ using Flutter

