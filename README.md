# 🔄 Unit Converter App – .NET MAUI

A simple and intuitive **Unit Converter** app built with **.NET MAUI (Multi-platform App UI)**. This cross-platform application allows users to convert units across categories like **length**, **weight**, **temperature**, and more.

---

## ✨ Features

- 🔢 **Unit Conversion**: Seamlessly convert units such as:
  - Meters ↔️ Kilometers  
  - Celsius ↔️ Fahrenheit  
  - Grams ↔️ Kilograms  
- 🧭 **User-Friendly Interface**: Clean and responsive design for an effortless conversion experience.

---

## 🛠️ Technologies Used

- 💻 **.NET MAUI** — Framework for building cross-platform apps with a single codebase  
- 🧠 **C#** — Application logic and core functionality  
- 🎨 **XAML** — UI layout and component design  
- 🔄 **MVU (Model-View-Update)** — Architecture pattern for managing state and UI updates efficiently

## Build and run

The committed project is `Mid_Project/Mid_Project.csproj`, targeting **.NET 9 MAUI** for Android, iOS, Mac Catalyst, and Windows (Windows target is included only on Windows). Use a matching .NET 9 SDK/MAUI toolchain; installing a newer SDK alone does not retarget this project.

Install the platform tools for your target: Android SDK/emulator for Android, Xcode on macOS for iOS/Mac Catalyst, or the Windows development tools for Windows. iOS device builds also require Apple signing configuration.

```bash
git clone https://github.com/NiraphatK/unit-converter-app.git
cd unit-converter-app
dotnet workload restore Mid_Project/Mid_Project.csproj
dotnet restore Mid_Project/Mid_Project.csproj
```

For Android with an emulator/device available:

```bash
dotnet build Mid_Project/Mid_Project.csproj -f net9.0-android -t:Run
```

For Mac Catalyst on macOS:

```bash
dotnet build Mid_Project/Mid_Project.csproj -f net9.0-maccatalyst -t:Run
```

For Windows on Windows:

```powershell
dotnet build Mid_Project/Mid_Project.csproj -f net9.0-windows10.0.19041.0 -t:Run
```

Alternatively, open `Mid_Project.sln` in a compatible MAUI IDE and select a supported target. Test a known conversion, such as 1 kilometer to 1,000 meters, and inspect conversion history. No automated test command is defined in this repository; platform builds and device behavior require verification on the corresponding host.
