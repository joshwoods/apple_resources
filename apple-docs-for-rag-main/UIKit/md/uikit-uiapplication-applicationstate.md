

- UIKit
- UIApplication
-  applicationState 

Instance Property

# applicationState

The app’s current state, or that of its most active scene.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var applicationState: UIApplication.State { get }
```

## Discussion

The behavior of this property depends on whether your app is scene-based.

In a scene-based app, this property takes the value of the most active scene, which it determines from each scene’s activationState property. A scene-based app launches in the background state, and transitions between its states as scenes connect, change their states, and disconnect. For scene-based apps, use UISceneDelegate to respond to changes in an individual scene’s life cycle.

In a sceneless app, the property’s value is always the app’s current state. The app is inactive at launch, and then is generally in either an active or background state. The app may become inactive for a short period — for example, when transitioning between active and background states, when the system presents an alert in front of it, or when the system displays the application switcher. For sceneless apps, use UIApplicationDelegate to respond to the app’s life cycle changes.

## See Also

### Getting the application state

enum State

Constants that indicate the running states of an app.

