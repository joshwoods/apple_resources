

- Quartz
- IKImageBrowserView
-  cellForItem(at:) 

Instance Method

# cellForItem(at:)

Returns the browser cell for the item at the specified index.

macOS 10.4+

``` source
@MainActor
func cellForItem(at index: Int) -> IKImageBrowserCell!
```

## Parameters 

`index`  

The index.

## Return Value

The browser cell at the specified index.

## Discussion

Subclasses must not override this method.

## See Also

### Getting Item Information

func indexOfItem(at: NSPoint) -> Int

Returns the index of the item at the specified location.

func itemFrame(at: Int) -> NSRect

Returns the frame rectangle for the item located at the specified index.

func visibleItemIndexes() -> IndexSet!

Returns the indexes of the view’s currently visible items.

