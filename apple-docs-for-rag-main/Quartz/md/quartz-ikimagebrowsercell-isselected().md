

- Quartz
- IKImageBrowserCell
-  isSelected() 

Instance Method

# isSelected()

Returns whether the cell is selected.

macOS 10.4+

``` source
func isSelected() -> Bool
```

## Return Value

true if the cell is selected, otherwise false.

## Discussion

Subclasses should not override this method.

## See Also

### Selection Handling

func selectionFrame() -> NSRect

Returns the receiver’s selection frame rectangle, which defines the position of the selection rectangle in its IKImageBrowserView.

