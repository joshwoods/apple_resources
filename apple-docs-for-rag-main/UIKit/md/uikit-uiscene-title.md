

- UIKit
- UIScene
-  title 

Instance Property

# title

A user-visible string you supply to help users differentiate among your app’s scenes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var title: String! { get set }
```

## Discussion

The system displays this string in the app switcher to make it easier for the user to differentiate among your app’s scenes. Set this property to an empty string if you don’t want the app switcher to display anything for the scene.

iPad and iPhone apps running on a Mac with Apple silicon and apps built with Mac Catalyst display the title in the title bar of the scene’s window.

## See Also

### Getting the scene attributes

var activationState: UIScene.ActivationState

The current execution state of the scene.

enum ActivationState

Constants that indicate the foreground or background execution state of your app.

var subtitle: String

A string that the app displays in the title bar of a window when running in macOS.

