

- Quartz
- IKImageBrowserView
-  contentResizingMask() 

Instance Method

# contentResizingMask()

Returns the receiver’s content resizing mask, which determines how its content is resized while zooming.

macOS 10.4+

``` source
@MainActor
func contentResizingMask() -> Int
```

## Return Value

The content resizing mask.

## See Also

### Zooming and Resizing

func setZoomValue(Float)

Sets the zoom value.

func zoomValue() -> Float

Returns the current zoom value.

func setContentResizingMask(Int)

Determines how the receiver resizes its content when zooming.

