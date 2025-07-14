

- Core Text
-  CTLineGetTrailingWhitespaceWidth(\_:) 

Function

# CTLineGetTrailingWhitespaceWidth(\_:)

Returns the trailing whitespace width for a line.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetTrailingWhitespaceWidth(_ line: CTLine) -> Double
```

## Parameters 

`line`  

The line whose trailing whitespace width is calculated.

## Return Value

The width of the line’s trailing whitespace. If the line is invalid, this function will always return zero.

## Discussion

Creating a line for a width can result in a line that is actually longer than the desired width due to trailing whitespace. Although this is typically not an issue due to whitespace being invisible, this function can be used to determine what amount of a line’s width is due to trailing whitespace.

## See Also

### Measuring Lines

func CTLineGetImageBounds(CTLine, CGContext?) -> CGRect

Calculates the image bounds for a line.

func CTLineGetTypographicBounds(CTLine, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Calculates the typographic bounds of a line.

