

- Quartz
- IKImageBrowserView
-  itemFrame(at:) 

Instance Method

# itemFrame(at:)

Returns the frame rectangle for the item located at the specified index.

macOS 10.4+

``` source
@MainActor
func itemFrame(at index: Int) -> NSRect
```

## Parameters 

`index`  

The index of the item whose frame rectangle you want to obtain.

## Return Value

The frame rectangle of the item.

## See Also

### Getting Item Information

func indexOfItem(at: NSPoint) -> Int

Returns the index of the item at the specified location.

func visibleItemIndexes() -> IndexSet!

Returns the indexes of the view’s currently visible items.

func cellForItem(at: Int) -> IKImageBrowserCell!

Returns the browser cell for the item at the specified index.

