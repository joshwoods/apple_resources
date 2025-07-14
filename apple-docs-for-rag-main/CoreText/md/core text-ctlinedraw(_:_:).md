

- Core Text
-  CTLineDraw(\_:\_:) 

Function

# CTLineDraw(\_:\_:)

Draws a complete line.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineDraw(
    _ line: CTLine,
    _ context: CGContext
)
```

## Parameters 

`line`  

The line to draw.

`context`  

The context into which the line is drawn.

## Discussion

This is a convenience function because the line could be drawn run-by-run by getting the glyph runs, getting the glyphs out of them, and calling a function such as CGContextShowGlyphsAtPositions. This call can leave the graphics context in any state and does not flush the context after the draw operation.

