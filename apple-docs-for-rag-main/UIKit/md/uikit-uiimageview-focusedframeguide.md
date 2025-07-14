

- UIKit
- UIImageView
-  focusedFrameGuide 

Instance Property

# focusedFrameGuide

The layout guide to use when the image view is focused.

tvOS 9.0+

``` source
@MainActor
var focusedFrameGuide: UILayoutGuide { get }
```

## Discussion

The layout guide in this property represents the display frame of the image view when it’s focused. You can use this property to align other elements of your interface to the image view or to adjust the constraints of your interface.

When the adjustsImageWhenAncestorFocused property is set to true, the image view automatically applies this layout guide when the image view becomes focused.

## See Also

### Managing focus-related behaviors

var adjustsImageWhenAncestorFocused: Bool

Allows UIImageView to respond when an ancestor becomes focused.

var masksFocusEffectToContents: Bool

A Boolean value indicating whether the floating focused appearance uses the image’s alpha channel.

