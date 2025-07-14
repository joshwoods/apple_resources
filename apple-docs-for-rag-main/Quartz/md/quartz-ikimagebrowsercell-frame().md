

- Quartz
- IKImageBrowserCell
-  frame() 

Instance Method

# frame()

Returns the receiver’s frame rectangle, which defines its position in its IKImageBrowserView.

macOS 10.4+

``` source
func frame() -> NSRect
```

## Return Value

The coordinates of the frame, in the `IKImageBrowserView` coordinate space.

## Discussion

Subclasses should not override this method.

## See Also

### Cell Component Frames

func imageFrame() -> NSRect

Returns the receiver’s image frame rectangle, which defines the position of the thumbnail in its IKImageBrowserView.

func subtitleFrame() -> NSRect

Returns the receiver’s subtitle frame rectangle.

func titleFrame() -> NSRect

Returns the receiver’s title frame rectangle.

func imageContainerFrame() -> NSRect

Returns the receiver’s image container frame rectangle, which defines the position of the container of the thumbnail.

