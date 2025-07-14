

- Core Text
-  kCTFrameClippingPathsAttributeName 

Global Variable

# kCTFrameClippingPathsAttributeName

Specifies array of paths to clip frame.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFrameClippingPathsAttributeName: CFString
```

## Discussion

The value must be a `CFArrayRef` containing `CFDictionaryRef`s. Each dictionary should have a `kCTFramePathClippingPathAttributeName` key-value pair, and can have a `kCTFramePathFillRuleAttributeName` key-value pair and `kCTFramePathFillRuleAttributeName` key-value pair as optional parameters.

## See Also

### Constants

enum CTFrameProgression

Constants that specify frame progression types.

let kCTFrameProgressionAttributeName: CFString

Specifies progression for a frame.

let kCTFramePathFillRuleAttributeName: CFString

The key used to specify the fill rule for a frame.

let kCTFramePathWidthAttributeName: CFString

The key used to specify the frame width.

let kCTFramePathClippingPathAttributeName: CFString

Specifies clipping path.

