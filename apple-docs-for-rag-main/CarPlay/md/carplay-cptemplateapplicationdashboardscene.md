

- CarPlay
-  CPTemplateApplicationDashboardScene 

Class

# CPTemplateApplicationDashboardScene

A CarPlay scene that controls your app’s dashboard navigation window.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
@MainActor
class CPTemplateApplicationDashboardScene
```

## Overview

A dashboard scene manages the display of your navigation app’s dashboard window on the CarPlay Dashboard, and notifies its delegate—an object that conforms to CPTemplateApplicationDashboardSceneDelegate—about scene life-cycle events. Use the dashboard controller the scene provides to supply shortcut buttons to display when there’s no active navigation session, further customizing you app’s presence on the CarPlay Dashboard.

You don’t create an instance of the dashboard scene directly. Instead, you specify the name of the class as part of the CarPlay Dashboard scene configuration that you add to your `Info.plist` file—see the example below—or that you return from your app delegate’s application(_:configurationForConnecting:options:) method.

```
```

## Topics

### Responding to the Dashboard Scene Life Cycle

var delegate: (any CPTemplateApplicationDashboardSceneDelegate)?

The object that receives the dashboard scene’s life-cycle events.

protocol CPTemplateApplicationDashboardSceneDelegate

The methods for responding to the life-cycle events of your navigation app’s dashboard scene.

### Accessing the Dashboard Controller

var dashboardController: CPDashboardController

The controller that manages the dashboard scene’s shortcut buttons.

class CPDashboardController

A controller that provides shortcut buttons for the CarPlay Dashboard.

### Accessing the Dashboard Window

var dashboardWindow: UIWindow

The window that belongs to the dashboard scene.

## Relationships

### Inherits From

- UIScene

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Navigation

Integrating CarPlay with Your Navigation App

Configure your navigation app to work with CarPlay by displaying your custom map and directions.

protocol CPTemplateApplicationDashboardSceneDelegate

The methods for responding to the life-cycle events of your navigation app’s dashboard scene.

class CPMapTemplate

A template that displays a navigation overlay that your app draws on the map.

class CPSearchTemplate

A template that provides the ability to search for a destination and see a list of search results.

class CPVoiceControlTemplate

A template that displays a voice control indicator during audio input.

