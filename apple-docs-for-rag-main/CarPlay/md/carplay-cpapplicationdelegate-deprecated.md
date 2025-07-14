

- CarPlay
-  CPApplicationDelegate Deprecated

Protocol

# CPApplicationDelegate

The interface for handling CarPlay life-cycle events.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
protocol CPApplicationDelegate : UIApplicationDelegate
```

## Overview

You must implement CPApplicationDelegate on the same object that serves as the delegate to your app.

## Topics

### Connecting to the CarPlay Interface

func application(UIApplication, didConnectCarInterfaceController: CPInterfaceController, to: CPWindow)

Tells the app delegate that the app connected to the CarPlay interface.

**Required**

func application(UIApplication, didDisconnectCarInterfaceController: CPInterfaceController, from: CPWindow)

Tells the app delegate that the app disconnected from the CarPlay interface.

**Required**

### Receiving the Selected Maneuver

func application(UIApplication, didSelect: CPManeuver)

Tells the app delegate that the user selected a maneuver.

### Handling Navigation Alert Actions

func application(UIApplication, didSelect: CPNavigationAlert)

Tells the app delegate that the user selected an action from a navigation alert.

## Relationships

### Inherits From

- NSObjectProtocol
- UIApplicationDelegate

