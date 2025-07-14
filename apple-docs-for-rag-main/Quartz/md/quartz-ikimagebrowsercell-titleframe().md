

- Quartz
- IKImageBrowserCell
-  titleFrame() 

Instance Method

# titleFrame()

Returns the receiver’s title frame rectangle.

macOS 10.4+

``` source
func titleFrame() -> NSRect
```

## Return Value

The coordinates of the title frame, in the `IKImageBrowserView` coordinate space.

## Discussion

It is the developer’s responsibility to compute the `titleFrame` such that it lies entirely within the cell’s frame() rectangle.

Subclasses can override this method to customize the position of the title.

## See Also

### Cell Component Frames

func frame() -> NSRect

Returns the receiver’s frame rectangle, which defines its position in its IKImageBrowserView.

func imageFrame() -> NSRect

Returns the receiver’s image frame rectangle, which defines the position of the thumbnail in its IKImageBrowserView.

func subtitleFrame() -> NSRect

Returns the receiver’s subtitle frame rectangle.

func imageContainerFrame() -> NSRect

Returns the receiver’s image container frame rectangle, which defines the position of the container of the thumbnail.

