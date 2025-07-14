

- Core Text
-  CTFrameGetStringRange(\_:) 

Function

# CTFrameGetStringRange(\_:)

Returns the range of characters originally requested to fill the frame.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFrameGetStringRange(_ frame: CTFrame) -> CFRange
```

## Parameters 

`frame`  

The frame whose character range is returned.

## Return Value

A `CFRange` structure containing the backing store range of characters that were originally requested to fill the frame, or, if the function call is not successful, an empty range.

## See Also

### Getting Frame Data

func CTFrameGetVisibleStringRange(CTFrame) -> CFRange

Returns the range of characters that actually fit in the frame.

func CTFrameGetPath(CTFrame) -> CGPath

Returns the path used to create the frame.

func CTFrameGetFrameAttributes(CTFrame) -> CFDictionary?

Returns the frame attributes used to create the frame.

