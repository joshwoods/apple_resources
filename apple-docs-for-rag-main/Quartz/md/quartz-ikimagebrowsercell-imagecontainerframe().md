

- Quartz
- IKImageBrowserCell
-  imageContainerFrame() 

Instance Method

# imageContainerFrame()

Returns the receiver’s image container frame rectangle, which defines the position of the container of the thumbnail.

macOS 10.4+

``` source
func imageContainerFrame() -> NSRect
```

## Return Value

The coordinates of image container frame, in the `IKImageBrowserView` coordinate space.

## Discussion

The image frame is computed automatically from the image container frame by taking in account the image alignment and the image aspect ratio.

Subclasses can override this method to customize the position of the thumbnail container.

## See Also

### Cell Component Frames

func frame() -> NSRect

Returns the receiver’s frame rectangle, which defines its position in its IKImageBrowserView.

func imageFrame() -> NSRect

Returns the receiver’s image frame rectangle, which defines the position of the thumbnail in its IKImageBrowserView.

func subtitleFrame() -> NSRect

Returns the receiver’s subtitle frame rectangle.

func titleFrame() -> NSRect

Returns the receiver’s title frame rectangle.

