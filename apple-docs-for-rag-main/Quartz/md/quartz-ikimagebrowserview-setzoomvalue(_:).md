

- Quartz
- IKImageBrowserView
-  setZoomValue(\_:) 

Instance Method

# setZoomValue(\_:)

Sets the zoom value.

macOS 10.4+

``` source
@MainActor
func setZoomValue(_ aValue: Float)
```

## Parameters 

`aValue`  

The zoom value. This value should be greater or equal to zero and less or equal than one. A zoom value of zero corresponds to the minimum size (40x40 pixels). A zoom value of one means images fits the browser bounds. Other values are interpolated.

## Discussion

You must use `setZoomValue` or setCellSize(_:), but not both. Setting the zoom value changes the cell size, and vice versa.

## See Also

### Related Documentation

func setCellSize(NSSize)

Sets the cell size.

### Zooming and Resizing

func zoomValue() -> Float

Returns the current zoom value.

func setContentResizingMask(Int)

Determines how the receiver resizes its content when zooming.

func contentResizingMask() -> Int

Returns the receiver’s content resizing mask, which determines how its content is resized while zooming.

