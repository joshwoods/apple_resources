

- SwiftUI
-  WKNotificationScene 

Structure

# WKNotificationScene

A scene which appears in response to receiving the specified category of remote or local notifications.

watchOS 7.0+

``` source
struct WKNotificationScene where Content : View, Controller : WKUserNotificationHostingController
```

## Mentioned in 

Declaring a custom view

## Topics

### Creating a notification scene

init(controller: Controller.Type, category: String)

Creates a scene that appears in response to receiving a specific category of remote or local notifications.

## Relationships

### Conforms To

- Scene

