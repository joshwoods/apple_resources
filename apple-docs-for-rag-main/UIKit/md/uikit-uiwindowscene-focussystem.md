

- UIKit
- UIWindowScene
-  focusSystem 

Instance Property

# focusSystem

The focus system that’s responsible for the window scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var focusSystem: UIFocusSystem? { get }
```

## Discussion

The value of this property is `nil` if the window scene doesn’t support focus.

