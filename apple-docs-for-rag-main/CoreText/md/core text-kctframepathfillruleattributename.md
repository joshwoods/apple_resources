

- Core Text
-  kCTFramePathFillRuleAttributeName 

Global Variable

# kCTFramePathFillRuleAttributeName

The key used to specify the fill rule for a frame.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFramePathFillRuleAttributeName: CFString
```

## Discussion

The value must be a CFNumber object containing a CTFramePathFillRule constant. The default value is CTFramePathFillRule.evenOdd.

## See Also

### Constants

enum CTFrameProgression

Constants that specify frame progression types.

let kCTFrameProgressionAttributeName: CFString

Specifies progression for a frame.

let kCTFramePathWidthAttributeName: CFString

The key used to specify the frame width.

let kCTFrameClippingPathsAttributeName: CFString

Specifies array of paths to clip frame.

let kCTFramePathClippingPathAttributeName: CFString

Specifies clipping path.

