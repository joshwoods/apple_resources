

- Quartz
- IKImageView
-  zoomImage(to:) 

Instance Method

# zoomImage(to:)

Zooms the image so that it fits in the specified rectangle.

macOS 10.5+

``` source
@MainActor
func zoomImage(to rect: NSRect)
```

## Parameters 

`rect`  

The rectangle to fit the image in.

## See Also

### Manipulating the Image in a View

func setRotationAngle(CGFloat, center: NSPoint)

Sets the rotation angle at the provided origin.

func setImageZoomFactor(CGFloat, center: NSPoint)

Sets the zoom factor at the provided origin.

func zoomImageToFit(Any!)

Zooms the image so that it fits in the image view.

func zoomImageToActualSize(Any!)

Zooms the image so that it is displayed using its true size.

func zoomIn(Any!)

Zooms the image in.

func zoomOut(Any!)

Zooms the image out.

func crop(Any!)

Crops the image using the current selection.

func flipImageHorizontal(Any!)

Flips an image along the horizontal axis.

func flipImageVertical(Any!)

Flips an image along the vertical axis.

func rotateImageLeft(Any!)

Rotates the image left (counter-clockwise).

func rotateImageRight(Any!)

Rotates the image right (clockwise).

