

- Quartz
- IKImageBrowserView
-  setCellSize(\_:) 

Instance Method

# setCellSize(\_:)

Sets the cell size.

macOS 10.4+

``` source
@MainActor
func setCellSize(_ size: NSSize)
```

## Parameters 

`size`  

The size to set.

## Discussion

You must use `setCellSize` or setZoomValue(_:), but not both. Setting the zoom value changes the cell size, and vice versa.

## See Also

### Related Documentation

func setZoomValue(Float)

Sets the zoom value.

### Setting and Getting Cell Size

func cellSize() -> NSSize

Returns the cell size.

