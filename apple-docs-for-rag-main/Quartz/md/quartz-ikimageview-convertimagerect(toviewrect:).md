

- Quartz
- IKImageView
-  convertImageRect(toViewRect:) 

Instance Method

# convertImageRect(toViewRect:)

Converts an image rectangle to an image view rectangle.

macOS 10.5+

``` source
@MainActor
func convertImageRect(toViewRect imageRect: NSRect) -> NSRect
```

## Parameters 

`imageRect`  

An rectangle specified in coordinates relative to the image.

## Return Value

An rectangle specified in coordinates relative to the image view.

## See Also

### Converting Points and Rectangles

func convertPoint(toImagePoint: NSPoint) -> NSPoint

Converts an image view coordinate to an image coordinate.

func convertRect(toImageRect: NSRect) -> NSRect

Converts an image view rectangle to an image rectangle.

func convertImagePoint(toViewPoint: NSPoint) -> NSPoint

Converts an image coordinate to an image view coordinate.

