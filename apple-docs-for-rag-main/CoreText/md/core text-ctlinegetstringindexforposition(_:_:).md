

- Core Text
-  CTLineGetStringIndexForPosition(\_:\_:) 

Function

# CTLineGetStringIndexForPosition(\_:\_:)

Performs hit testing.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetStringIndexForPosition(
    _ line: CTLine,
    _ position: CGPoint
) -> CFIndex
```

## Parameters 

`line`  

The line being examined.

`position`  

The location of the mouse click relative to the line’s origin.

## Return Value

The string index for the position, or if the line does not support string access, kCFNotFound. Relative to the line’s string range, this value can be no less than the first string index and no greater than the last string index plus 1.

## Discussion

This function can be used to determine the string index for a mouse click or other event. This string index corresponds to the character before which the next character should be inserted. This determination is made by analyzing the string from which a typesetter was created and the corresponding glyphs as embodied by a particular line.

## See Also

### Getting Line Positioning

func CTLineGetOffsetForStringIndex(CTLine, CFIndex, UnsafeMutablePointer&lt;CGFloat>?) -> CGFloat

Determines the graphical offset or offsets for a string index.

func CTLineEnumerateCaretOffsets(CTLine, (Double, CFIndex, Bool, UnsafeMutablePointer&lt;Bool>) -> Void)

Enumerates caret offsets for characters in a line.

