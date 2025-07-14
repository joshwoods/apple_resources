

- Quartz
- IKImageBrowserView
-  setContentResizingMask(\_:) 

Instance Method

# setContentResizingMask(\_:)

Determines how the receiver resizes its content when zooming.

macOS 10.4+

``` source
@MainActor
func setContentResizingMask(_ mask: Int)
```

## Parameters 

`mask`  

A resizing mask. You specify a mask by combining any of the following options using the C bitwise `OR` operator: width, height. Other values are ignored.

## See Also

### Zooming and Resizing

func setZoomValue(Float)

Sets the zoom value.

func zoomValue() -> Float

Returns the current zoom value.

func contentResizingMask() -> Int

Returns the receiver’s content resizing mask, which determines how its content is resized while zooming.

