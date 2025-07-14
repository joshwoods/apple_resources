

- UIKit
- UIApplicationDelegate
-  window 

Instance Property

# window

The window to use when presenting a storyboard.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional var window: UIWindow? { get set }
```

## Discussion

This property contains the window used to present the app’s visual content on the device’s main screen.

Implementation of this property is required if your app’s `Info.plist` file contains the `UIMainStoryboardFile` key. Fortunately, the Xcode project templates usually include a synthesized declaration of the property automatically for the app delegate. The default value of this synthesized property is `nil`, which causes the app to create a generic UIWindow object and assign it to the property. If you want to provide a custom window for your app, you must implement the getter method of this property and use it to create and return your custom window.

For more information about the UIMainStoryboardFile key, see Information Property List Key Reference.

