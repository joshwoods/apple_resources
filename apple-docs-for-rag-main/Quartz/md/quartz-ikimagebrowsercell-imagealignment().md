

- Quartz
- IKImageBrowserCell
-  imageAlignment() 

Instance Method

# imageAlignment()

Returns the position of the cell’s image in the frame.

macOS 10.4+

``` source
func imageAlignment() -> NSImageAlignment
```

## Return Value

The alignment of the image. See NSImageAlignment for possible values.

## Discussion

Subclasses can override this method to customize the image alignment.

The image frame will be computed automatically from the image container frame by taking in account the image alignment and the image aspect ratio.

## See Also

### Cell Content Display

func opacity() -> CGFloat

Returns the opacity of the receiver.

