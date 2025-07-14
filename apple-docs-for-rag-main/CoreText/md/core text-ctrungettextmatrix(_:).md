

- Core Text
-  CTRunGetTextMatrix(\_:) 

Function

# CTRunGetTextMatrix(\_:)

Returns the text matrix needed to draw this run.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetTextMatrix(_ run: CTRun) -> CGAffineTransform
```

## Parameters 

`run`  

The run object from which to get the text matrix.

## Return Value

A CGAffineTransform structure.

## Discussion

To properly draw the glyphs in a run, the fields `tx` and `ty` of the CGAffineTransform returned by this function should be set to the current text position.

## See Also

### Drawing the Glyph Run

func CTRunDraw(CTRun, CGContext, CFRange)

Draws a complete run or part of one.

