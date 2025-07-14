

- Core Text
-  kCTFrameProgressionAttributeName 

Global Variable

# kCTFrameProgressionAttributeName

Specifies progression for a frame.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFrameProgressionAttributeName: CFString
```

## Discussion

A CFNumber object containing a CTFrameProgression constant. The default is `kCTFrameProgressionTopToBottom`.

This value determines the line-stacking behavior for a frame and does not affect the appearance of the glyphs within that frame.

## See Also

### Constants

enum CTFrameProgression

Constants that specify frame progression types.

let kCTFramePathFillRuleAttributeName: CFString

The key used to specify the fill rule for a frame.

let kCTFramePathWidthAttributeName: CFString

The key used to specify the frame width.

let kCTFrameClippingPathsAttributeName: CFString

Specifies array of paths to clip frame.

let kCTFramePathClippingPathAttributeName: CFString

Specifies clipping path.

