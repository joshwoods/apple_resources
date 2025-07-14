

- Core Text
-  kCTFramePathClippingPathAttributeName 

Global Variable

# kCTFramePathClippingPathAttributeName

Specifies clipping path.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFramePathClippingPathAttributeName: CFString
```

## Discussion

Specifies clipping path. This attribute is valid only in a dictionary contained in an array specified by `kCTFrameClippingPathsAttributeName`.

The value must be a `CGPathRef` specifying a clipping path. See kCTFrameClippingPathsAttributeName.

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

let kCTFrameClippingPathsAttributeName: CFString

Specifies array of paths to clip frame.

