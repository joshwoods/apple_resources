

- Core Text
-  CTLineGetImageBounds(\_:\_:) 

Function

# CTLineGetImageBounds(\_:\_:)

Calculates the image bounds for a line.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetImageBounds(
    _ line: CTLine,
    _ context: CGContext?
) -> CGRect
```

## Parameters 

`line`  

The line whose image bounds are calculated.

`context`  

The context for which the image bounds are calculated. This is required because the context could have settings in it that would cause changes in the image bounds.

## Return Value

A rectangle that tightly encloses the paths of the line’s glyphs, or, if the line or context is invalid, CGRectNull.

## See Also

### Measuring Lines

func CTLineGetTypographicBounds(CTLine, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Calculates the typographic bounds of a line.

func CTLineGetTrailingWhitespaceWidth(CTLine) -> Double

Returns the trailing whitespace width for a line.

