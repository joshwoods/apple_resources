

- UIKit
- UIImageView
-  masksFocusEffectToContents 

Instance Property

# masksFocusEffectToContents

A Boolean value indicating whether the floating focused appearance uses the image’s alpha channel.

tvOS 11.0+

``` source
@MainActor
var masksFocusEffectToContents: Bool { get set }
```

## Discussion

Set this property to false when using multi-layer images or when using images that are completely opaque. Set this property to true only when the image view contains a single-layer image with transparency. When set to true, the system uses the image’s alpha channel to create an appropriate floating focused appearance. For example, the system masks the shadow based on the alpha channel of the image.

The aspect ratio of the image view and its displayed image must be the same. Rendering with transparency affects performance, so enable this option only when needed.

## See Also

### Managing focus-related behaviors

var adjustsImageWhenAncestorFocused: Bool

Allows UIImageView to respond when an ancestor becomes focused.

var focusedFrameGuide: UILayoutGuide

The layout guide to use when the image view is focused.

