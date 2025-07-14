

- Core Text
-  CTFrameGetPath(\_:) 

Function

# CTFrameGetPath(\_:)

Returns the path used to create the frame.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFrameGetPath(_ frame: CTFrame) -> CGPath
```

## Parameters 

`frame`  

The frame whose path is returned.

## See Also

### Getting Frame Data

func CTFrameGetStringRange(CTFrame) -> CFRange

Returns the range of characters originally requested to fill the frame.

func CTFrameGetVisibleStringRange(CTFrame) -> CFRange

Returns the range of characters that actually fit in the frame.

func CTFrameGetFrameAttributes(CTFrame) -> CFDictionary?

Returns the frame attributes used to create the frame.

