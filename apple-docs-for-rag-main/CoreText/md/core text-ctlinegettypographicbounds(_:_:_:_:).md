

- Core Text
-  CTLineGetTypographicBounds(\_:\_:\_:\_:) 

Function

# CTLineGetTypographicBounds(\_:\_:\_:\_:)

Calculates the typographic bounds of a line.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetTypographicBounds(
    _ line: CTLine,
    _ ascent: UnsafeMutablePointer?,
    _ descent: UnsafeMutablePointer?,
    _ leading: UnsafeMutablePointer?
) -> Double
```

## Parameters 

`line`  

The line whose typographic bounds are calculated.

`ascent`  

On output, the ascent of the line. This parameter can be set to `NULL` if not needed.

`descent`  

On output, the descent of the line. This parameter can be set to `NULL` if not needed.

`leading`  

On output, the leading of the line. This parameter can be set to `NULL` if not needed.

## Return Value

The typographic width of the line. If the line is invalid, this function returns `0`.

## See Also

### Measuring Lines

func CTLineGetImageBounds(CTLine, CGContext?) -> CGRect

Calculates the image bounds for a line.

func CTLineGetTrailingWhitespaceWidth(CTLine) -> Double

Returns the trailing whitespace width for a line.

