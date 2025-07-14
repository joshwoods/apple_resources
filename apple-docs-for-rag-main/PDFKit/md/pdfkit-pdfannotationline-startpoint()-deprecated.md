

- PDFKit
- PDFAnnotationLine
-  startPoint() Deprecated

Instance Method

# startPoint()

Returns the starting point for the line.

macOS 10.4–10.12Deprecated

``` source
func startPoint() -> NSPoint
```

## Return Value

The starting point for the line, in page space.

## Discussion

Page space is a 72-dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Specifying the Starting and Ending Points

func setStart(NSPoint)

Sets the starting point for the line.

Deprecated

func endPoint() -> NSPoint

Returns the ending point for the line in page space.

Deprecated

func setEnd(NSPoint)

Sets the ending point for the line.

Deprecated

