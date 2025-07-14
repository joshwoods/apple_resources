

- Core Text
-  CTFrameGetLines(\_:) 

Function

# CTFrameGetLines(\_:)

Returns an array of lines stored in the frame.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFrameGetLines(_ frame: CTFrame) -> CFArray
```

## Parameters 

`frame`  

The frame whose line array is returned.

## Return Value

A CFArray object containing the CTLine objects that make up the frame, or, if there are no lines in the frame, an array with no elements.

## See Also

### Getting Lines

func CTFrameGetLineOrigins(CTFrame, CFRange, UnsafeMutablePointer&lt;CGPoint>)

Copies a range of line origins for a frame.

