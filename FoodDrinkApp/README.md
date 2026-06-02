# NutriTrack – Food & Drink Assistant

NutriTrack is a .NET MAUI project for my “Food and Drink” coursework. The app lets you log food and drink items, see nutrition summaries, validate user input, and demonstrate a bunch of mobile hardware features.


## What it does
- Browse a list of food & drink items, search for something, and open a detail page.

- Add new entries with a form that checks required fields and numeric values (e.g. calories).

- Take a photo of your meal using the camera, and preview it.

- Record where you ate or bought something using GPS/location.

- Use text‑to‑speech to read out nutrition info or help content.

- Vibrate or give haptic feedback when you perform certain actions.

- Switch between light/dark theme, and make text larger.

- Includes semantic labels, screen reader announcements, and clear validation messages.

## How it covers the marking criteria
- UI/UX & accessibility – XAML pages, bottom navigation bar, consistent colours, dark mode, semantic descriptions, and screen reader support.

- Mobile hardware – Camera, location, text‑to‑speech, vibration, haptic feedback.

- Functionality – List, search, add new items, detail view, settings page, hardware demo flows.

- Validation & error handling – Required field checks, numeric range checks, permission errors, friendly messages when hardware isn’t available.

- Code quality – Separated models and services, clear naming, reusable helpers, reasonably clean page‑level code.

- Deployment – Cross‑platform .NET MAUI app that runs on Android and Windows.

- GitHub usage – Regular commits throughout development, e.g. `Add food list page`, `Implement hardware page`, `Add input validation`.

## How to run it

Open `FoodDrinkApp.csproj` or `FoodDrinkApp.sln` in Visual Studio 2022 with the .NET MAUI workload installed.

Recommended targets for demonstrating:

- Android emulator

- Windows Machine

Build commands if you want to do it manually:

Windows:
```powershell
dotnet build .\FoodDrinkApp.csproj -f net9.0-windows10.0.19041.0
```

Android:

```powershell
dotnet build .\FoodDrinkApp.csproj -f net9.0-android
```

The project using `Directory.Build.props` to send build outputs to `C:\MauiBuild\NutriTrack\`,That’s just to avoid weird `asset` path issues on Android when the project is in a path containing Chinese characters.

## What to show in my screencast
Explain the “Food and Drink” theme and what NutriTrack does.

Show search, detail page, and adding a new record.

Demonstrate validation: leave a required field empty, enter an invalid number – show the error messages.

Show camera, location, text‑to‑speech, vibration, and haptic feedback.

Show dark mode and large font mode.

Show important code files: models, services, pages, and Android permission config.

Show the app running on Android and Windows.

Show GitHub commit history and this README.
