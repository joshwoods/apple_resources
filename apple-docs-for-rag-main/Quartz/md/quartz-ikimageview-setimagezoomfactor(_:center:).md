

- Quartz
- IKImageView
-  setImageZoomFactor(\_:center:) 

Instance Method

# setImageZoomFactor(\_:center:)

Sets the zoom factor at the provided origin.

macOS 10.5+

``` source
@MainActor
func setImageZoomFactor(
    _ zoomFactor: CGFloat,
    center centerPoint: NSPoint
)
```

## Parameters 

`zoomFactor`  

The zoom factor to apply to the image.

`centerPoint`  

The point that specifies the origin of the zoom factor.

## See Also

### Related Documentation

var zoomFactor: CGFloat

Specifies the zoom factor for the image view.

### Manipulating the Image in a View

func setRotationAngle(CGFloat, center: NSPoint)

Sets the rotation angle at the provided origin.

func zoomImageToFit(Any!)

Zooms the image so that it fits in the image view.

func zoomImageToActualSize(Any!)

Zooms the image so that it is displayed using its true size.

func zoomImage(to: NSRect)

Zooms the image so that it fits in the specified rectangle.

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

