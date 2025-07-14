

- SwiftUI
-  SettingsLink 

Structure

# SettingsLink

A view that opens the Settings scene defined by an app.

macOS 14.0+

``` source
struct SettingsLink where Label : View
```

## Overview

On macOS, clicking on the link opens the window for the scene or orders it to the front if it is already open.

## Topics

### Creating a settings link

init()

Creates a settings link with the default system label.

init(label: () -> Label)

Creates a settings link with a custom label.

### Supporting types

struct DefaultSettingsLinkLabel

The default label to use for a settings link.

## Relationships

### Conforms To

- View

## See Also

### Managing a settings window

struct Settings

A scene that presents an interface for viewing and modifying an app’s settings.

struct OpenSettingsAction

An action that presents the settings scene for an app.

var openSettings: OpenSettingsAction

A Settings presentation action stored in a view’s environment.

