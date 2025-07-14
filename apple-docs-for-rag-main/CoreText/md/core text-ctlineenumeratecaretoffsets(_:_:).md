

- Core Text
-  CTLineEnumerateCaretOffsets(\_:\_:) 

Function

# CTLineEnumerateCaretOffsets(\_:\_:)

Enumerates caret offsets for characters in a line.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineEnumerateCaretOffsets(
    _ line: CTLine,
    _ block: @escaping (Double, CFIndex, Bool, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`line`  

The line to enumerate.

`block`  

The block to invoke once for each logical caret edge in the line, in left-to-right visual order. The block’s `offset` parameter is relative to the line origin. The block’s `leadingEdge` parameter specifies logical order.

## See Also

### Getting Line Positioning

func CTLineGetStringIndexForPosition(CTLine, CGPoint) -> CFIndex

Performs hit testing.

func CTLineGetOffsetForStringIndex(CTLine, CFIndex, UnsafeMutablePointer&lt;CGFloat>?) -> CGFloat

Determines the graphical offset or offsets for a string index.

