

- PDFKit
- PDFAnnotationLine
-  endPoint() Deprecated

Instance Method

# endPoint()

Returns the ending point for the line in page space.

macOS 10.4–10.12Deprecated

``` source
func endPoint() -> NSPoint
```

## Return Value

The ending point for the line, in page space.

## Discussion

Page space is a 72-dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Specifying the Starting and Ending Points

func startPoint() -> NSPoint

Returns the starting point for the line.

Deprecated

func setStart(NSPoint)

Sets the starting point for the line.

Deprecated

func setEnd(NSPoint)

Sets the ending point for the line.

Deprecated

