

- Quartz
- IKImageBrowserCell
-  opacity() 

Instance Method

# opacity()

Returns the opacity of the receiver.

macOS 10.4+

``` source
func opacity() -> CGFloat
```

## Return Value

The cell’s opacity.

## Discussion

Possible values are between 0.0 (transparent) and 1.0 (opaque).

Subclasses can override this method to customize the opacity of the cell.

## See Also

### Cell Content Display

func imageAlignment() -> NSImageAlignment

Returns the position of the cell’s image in the frame.

