

- Quartz
- IKImageBrowserView
-  indexOfItem(at:) 

Instance Method

# indexOfItem(at:)

Returns the index of the item at the specified location.

macOS 10.4+

``` source
@MainActor
func indexOfItem(at point: NSPoint) -> Int
```

## Parameters 

`point`  

The location of the item.

## Return Value

The index of the item or `NSNotFound` if no item at this location.

## See Also

### Getting Item Information

func itemFrame(at: Int) -> NSRect

Returns the frame rectangle for the item located at the specified index.

func visibleItemIndexes() -> IndexSet!

Returns the indexes of the view’s currently visible items.

func cellForItem(at: Int) -> IKImageBrowserCell!

Returns the browser cell for the item at the specified index.

