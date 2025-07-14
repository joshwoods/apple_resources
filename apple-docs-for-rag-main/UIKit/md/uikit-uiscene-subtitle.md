

- UIKit
- UIScene
-  subtitle 

Instance Property

# subtitle

A string that the app displays in the title bar of a window when running in macOS.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var subtitle: String { get set }
```

## Discussion

When this property is an empty string, the system removes the subtitle from the window layout. The default value is an empty string.

Note

Apps running in iOS ignore the subtitle property.

## See Also

### Getting the scene attributes

var activationState: UIScene.ActivationState

The current execution state of the scene.

enum ActivationState

Constants that indicate the foreground or background execution state of your app.

var title: String!

A user-visible string you supply to help users differentiate among your app’s scenes.

