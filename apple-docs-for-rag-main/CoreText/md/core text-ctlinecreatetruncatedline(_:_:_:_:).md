

- Core Text
-  CTLineCreateTruncatedLine(\_:\_:\_:\_:) 

Function

# CTLineCreateTruncatedLine(\_:\_:\_:\_:)

Creates a truncated line from an existing line.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineCreateTruncatedLine(
    _ line: CTLine,
    _ width: Double,
    _ truncationType: CTLineTruncationType,
    _ truncationToken: CTLine?
) -> CTLine?
```

## Parameters 

`line`  

The line from which to create a truncated line.

`width`  

The width at which truncation begins. The line is truncated if its width is greater than the width passed in this parameter.

`truncationType`  

The type of truncation to perform if needed. See CTLineTruncationType for possible values.

`truncationToken`  

This token is added at the point where truncation took place, to indicate that the line was truncated. Usually, the truncation token is the ellipsis character (`U+2026`). If this parameter is set to `NULL`, then no truncation token is used and the line is simply cut off.

## Return Value

A reference to a truncated CTLine object if the call was successful; otherwise, `NULL`.

## Discussion

The line specified in `truncationToken` should have a width less than the width specified by the `width` parameter. If the width of the line specified in `truncationToken` is greater than `width` and truncation is needed, the function returns `NULL`.

## See Also

### Creating Lines

func CTLineCreateWithAttributedString(CFAttributedString) -> CTLine

Creates a single immutable line object from an attributed string.

func CTLineCreateJustifiedLine(CTLine, CGFloat, Double) -> CTLine?

Creates a justified line from an existing line.

