

- UIKit
- UIWindowScene
-  windows 

Instance Property

# windows

The windows associated with the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var windows: [UIWindow] { get }
```

## Discussion

Use this property to retrieve the windows associated with the scene. To remove the window from the current scene, or move it to a different scene, change the value of the window’s windowScene property.

## See Also

### Getting the active windows

var keyWindow: UIWindow?

The key window associated with the scene.

var screen: UIScreen

The screen that displays the contents of the scene.

