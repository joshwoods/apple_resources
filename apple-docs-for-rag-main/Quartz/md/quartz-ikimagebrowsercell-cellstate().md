

- Quartz
- IKImageBrowserCell
-  cellState() 

Instance Method

# cellState()

Returns the current cell state of the receiver.

macOS 10.4+

``` source
func cellState() -> IKImageBrowserCellState
```

## Return Value

The current state of the cell. See IKImageBrowserCellState for possible values.

## Discussion

The IKImageBrowserView creates thumbnails asynchronously. This method returns the current state.

