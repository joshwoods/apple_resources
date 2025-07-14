

- Quartz
- IKImageBrowserCell
-  imageFrame() 

Instance Method

# imageFrame()

Returns the receiver’s image frame rectangle, which defines the position of the thumbnail in its IKImageBrowserView.

macOS 10.4+

``` source
func imageFrame() -> NSRect
```

## Return Value

The coordinates of the frame, in the `IKImageBrowserView` coordinate space.

## Discussion

It is the developer’s responsibility to compute the `imageFrame` such that it lies entirely within the cell’s frame() rectangle.

Subclasses can override this method to customize the position of the thumbnail.

## See Also

### Cell Component Frames

func frame() -> NSRect

Returns the receiver’s frame rectangle, which defines its position in its IKImageBrowserView.

func subtitleFrame() -> NSRect

Returns the receiver’s subtitle frame rectangle.

func titleFrame() -> NSRect

Returns the receiver’s title frame rectangle.

func imageContainerFrame() -> NSRect

Returns the receiver’s image container frame rectangle, which defines the position of the container of the thumbnail.

