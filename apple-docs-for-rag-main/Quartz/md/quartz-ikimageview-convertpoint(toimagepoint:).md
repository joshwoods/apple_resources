

- Quartz
- IKImageView
-  convertPoint(toImagePoint:) 

Instance Method

# convertPoint(toImagePoint:)

Converts an image view coordinate to an image coordinate.

macOS 10.5+

``` source
@MainActor
func convertPoint(toImagePoint viewPoint: NSPoint) -> NSPoint
```

## Parameters 

`viewPoint`  

A point specified in coordinates relative to the image view.

## Return Value

The point specified in coordinates relative to the image.

## See Also

### Converting Points and Rectangles

func convertRect(toImageRect: NSRect) -> NSRect

Converts an image view rectangle to an image rectangle.

func convertImagePoint(toViewPoint: NSPoint) -> NSPoint

Converts an image coordinate to an image view coordinate.

func convertImageRect(toViewRect: NSRect) -> NSRect

Converts an image rectangle to an image view rectangle.

