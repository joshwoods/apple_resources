

- PDFKit
- PDFAnnotationLine
-  setStart(\_:) Deprecated

Instance Method

# setStart(\_:)

Sets the starting point for the line.

macOS 10.4–10.12Deprecated

``` source
func setStart(_ point: NSPoint)
```

## Parameters 

`point`  

The starting point for the line, in page space.

## Discussion

Page space is a 72-dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Specifying the Starting and Ending Points

func startPoint() -> NSPoint

Returns the starting point for the line.

Deprecated

func endPoint() -> NSPoint

Returns the ending point for the line in page space.

Deprecated

func setEnd(NSPoint)

Sets the ending point for the line.

Deprecated

