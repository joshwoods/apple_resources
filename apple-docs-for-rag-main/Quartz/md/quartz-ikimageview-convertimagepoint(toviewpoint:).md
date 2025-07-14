

- Quartz
- IKImageView
-  convertImagePoint(toViewPoint:) 

Instance Method

# convertImagePoint(toViewPoint:)

Converts an image coordinate to an image view coordinate.

macOS 10.5+

``` source
@MainActor
func convertImagePoint(toViewPoint imagePoint: NSPoint) -> NSPoint
```

## Parameters 

`imagePoint`  

A point specified in coordinates relative to the image.

## Return Value

A point specified in coordinates relative to the image view.

## See Also

### Converting Points and Rectangles

func convertPoint(toImagePoint: NSPoint) -> NSPoint

Converts an image view coordinate to an image coordinate.

func convertRect(toImageRect: NSRect) -> NSRect

Converts an image view rectangle to an image rectangle.

func convertImageRect(toViewRect: NSRect) -> NSRect

Converts an image rectangle to an image view rectangle.

