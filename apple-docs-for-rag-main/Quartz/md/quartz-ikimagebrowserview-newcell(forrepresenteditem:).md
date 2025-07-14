

- Quartz
- IKImageBrowserView
-  newCell(forRepresentedItem:) 

Instance Method

# newCell(forRepresentedItem:)

Returns the cell to use for the specified item.

macOS 10.4+

``` source
@MainActor
func newCell(forRepresentedItem anItem: Any!) -> IKImageBrowserCell!
```

## Parameters 

`anItem`  

The item that the returned cell will represent.

## Return Value

A new cell.

## Discussion

Subclasses can override this method to customize the appearance of the cell that will represent `anItem`.

