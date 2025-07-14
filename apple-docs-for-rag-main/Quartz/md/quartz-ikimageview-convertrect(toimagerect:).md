

- Quartz
- IKImageView
-  convertRect(toImageRect:) 

Instance Method

# convertRect(toImageRect:)

Converts an image view rectangle to an image rectangle.

macOS 10.5+

``` source
@MainActor
func convertRect(toImageRect viewRect: NSRect) -> NSRect
```

## Parameters 

`viewRect`  

An rectangle specified in coordinates relative to the image view.

## Return Value

The rectangle specified in coordinates relative to the image.

## See Also

### Converting Points and Rectangles

func convertPoint(toImagePoint: NSPoint) -> NSPoint

Converts an image view coordinate to an image coordinate.

func convertImagePoint(toViewPoint: NSPoint) -> NSPoint

Converts an image coordinate to an image view coordinate.

func convertImageRect(toViewRect: NSRect) -> NSRect

Converts an image rectangle to an image view rectangle.

