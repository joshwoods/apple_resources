

- Quartz
- IKImageBrowserCell
-  selectionFrame() 

Instance Method

# selectionFrame()

Returns the receiver’s selection frame rectangle, which defines the position of the selection rectangle in its IKImageBrowserView.

macOS 10.4+

``` source
func selectionFrame() -> NSRect
```

## Return Value

The cells selection frame, in the `IKImageBrowserView` coordinate space.

## Discussion

Subclasses can override this method to customize the position of the selection frame.

## See Also

### Selection Handling

func isSelected() -> Bool

Returns whether the cell is selected.

