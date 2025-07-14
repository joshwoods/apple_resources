

- Quartz
- IKImageView
-  rotateImageRight(\_:) 

Instance Method

# rotateImageRight(\_:)

Rotates the image right (clockwise).

macOS 10.5+

``` source
@IBAction @MainActor
func rotateImageRight(_ sender: Any!)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

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

