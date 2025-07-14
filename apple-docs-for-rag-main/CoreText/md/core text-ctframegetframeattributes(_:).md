

- Core Text
-  CTFrameGetFrameAttributes(\_:) 

Function

# CTFrameGetFrameAttributes(\_:)

Returns the frame attributes used to create the frame.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFrameGetFrameAttributes(_ frame: CTFrame) -> CFDictionary?
```

## Parameters 

`frame`  

The frame whose attributes are returned.

## Return Value

A reference to a CFDictionary object containing the frame attributes that were used to create the frame, or, if the frame was created without any frame attributes, `NULL`.

## Discussion

You can create a frame with an attributes dictionary to control various aspects of the framing process. These attributes are different from the ones used to create an attributed string.

## See Also

### Getting Frame Data

func CTFrameGetStringRange(CTFrame) -> CFRange

Returns the range of characters originally requested to fill the frame.

func CTFrameGetVisibleStringRange(CTFrame) -> CFRange

Returns the range of characters that actually fit in the frame.

func CTFrameGetPath(CTFrame) -> CGPath

Returns the path used to create the frame.

