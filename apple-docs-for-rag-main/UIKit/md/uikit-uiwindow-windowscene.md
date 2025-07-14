

- UIKit
- UIWindow
-  windowScene 

Instance Property

# windowScene

The scene containing the window.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
weak var windowScene: UIWindowScene? { get set }
```

## Discussion

Changing the value of this property moves the window to the newly specified scene. Setting the property to `nil` removes the window from its current scene.

## See Also

### Getting related objects

var avDisplayManager: AVDisplayManager

The display manager that handles requests for screen resolution, refresh rate, and HDR mode information.

