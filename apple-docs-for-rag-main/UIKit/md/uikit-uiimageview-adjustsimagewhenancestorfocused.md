

- UIKit
- UIImageView
-  adjustsImageWhenAncestorFocused 

Instance Property

# adjustsImageWhenAncestorFocused

Allows UIImageView to respond when an ancestor becomes focused.

tvOS 9.0+

``` source
@MainActor
var adjustsImageWhenAncestorFocused: Bool { get set }
```

## Discussion

When the value of this property is true and an ancestor of the image view becomes focused, the image view adjusts the frame of its image using the focusedFrameGuide property. The default value of this property is false.

## See Also

### Managing focus-related behaviors

var focusedFrameGuide: UILayoutGuide

The layout guide to use when the image view is focused.

var masksFocusEffectToContents: Bool

A Boolean value indicating whether the floating focused appearance uses the image’s alpha channel.

