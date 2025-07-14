

- SwiftUI
-  OpenSettingsAction 

Structure

# OpenSettingsAction

An action that presents the settings scene for an app.

macOS 14.0+

``` source
@MainActor @preconcurrency
struct OpenSettingsAction
```

## Overview

Use the openSettings environment value to get the instance of this structure for a given Environment. Then call the instance to open a window. You call the instance directly because it defines a callAsFunction() method that Swift calls when you call the instance.

For example, you can define a button that opens the settings window to a particular tab:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        #if os(macOS)
        Settings {
            SettingsView()
        }
        #endif
    }
}

struct SettingsView: View {
    @AppStorage("selectedSettingsTab")
    private var selectedSettingsTab = SettingsTab.general

    var body: some View {
        TabView(selection: $selectedSettingsTab) {
            GeneralSettings()
            AdvancedSettings()
        }
    }
}

struct AdvancedSettingsButton: View {
    @AppStorage("selectedSettingsTab")
    private var selectedSettingsTab = SettingsTab.general

    @Environment(\.openSettings) private var openSettings

    var body: some View {
        Button("Open Advanced Settings…") {
            selectedSettingsTab = .advanced
            openSettings()
        }
    }
}

enum SettingsTab: Int {
    case general
    case advanced
}
```

## Topics

### Instance Methods

func callAsFunction()

Opens the window associated to the Settings scene defined by this app, if one exists.

## Relationships

### Conforms To

- Sendable

## See Also

### Managing a settings window

struct Settings

A scene that presents an interface for viewing and modifying an app’s settings.

struct SettingsLink

A view that opens the Settings scene defined by an app.

var openSettings: OpenSettingsAction

A Settings presentation action stored in a view’s environment.

