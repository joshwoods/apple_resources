

- Quartz
- IKImageBrowserView
-  visibleItemIndexes() 

Instance Method

# visibleItemIndexes()

Returns the indexes of the view’s currently visible items.

macOS 10.4+

``` source
@MainActor
func visibleItemIndexes() -> IndexSet!
```

## Return Value

A set containing the indexes.

## See Also

### Getting Item Information

func indexOfItem(at: NSPoint) -> Int

Returns the index of the item at the specified location.

func itemFrame(at: Int) -> NSRect

Returns the frame rectangle for the item located at the specified index.

func cellForItem(at: Int) -> IKImageBrowserCell!

Returns the browser cell for the item at the specified index.

