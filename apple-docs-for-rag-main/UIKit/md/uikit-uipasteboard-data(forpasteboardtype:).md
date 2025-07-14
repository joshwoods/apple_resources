

- UIKit
- UIPasteboard
-  data(forPasteboardType:) 

Instance Method

# data(forPasteboardType:)

Returns the data on the pasteboard for the given representation type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func data(forPasteboardType pasteboardType: String) -> Data?
```

## Parameters 

`pasteboardType`  

A string identifying a representation type of a pasteboard item.

## Return Value

A data object or `nil` if there is no data in the pasteboard of the given type.

## Discussion

The returned object often holds raw (binary) data, such as image data. This method works on the first item in the pasteboard. If there are other items, it ignores them.

## See Also

### Getting and setting pasteboard items

var numberOfItems: Int

The number of items for the pasteboard.

var items: [[String : Any]]

The pasteboard items on the pasteboard.

func addItems([[String : Any]])

Appends pasteboard items to the current contents of the pasteboard.

func setItems([[String : Any]], options: [UIPasteboard.OptionsKey : Any])

Adds an array of items to a pasteboard, and sets privacy options for all the items on the pasteboard.

func data(forPasteboardType: String, inItemSet: IndexSet?) -> [Data]?

Returns the data objects in the indicated pasteboard items that have the given representation type.

func setData(Data, forPasteboardType: String)

Puts data on the pasteboard for the specified representation type.

func value(forPasteboardType: String) -> Any?

Returns an object on the pasteboard for the given representation type.

func values(forPasteboardType: String, inItemSet: IndexSet?) -> [Any]?

Returns the objects on the indicated pasteboard items that have the given representation type.

func setValue(Any, forPasteboardType: String)

Puts an object on the pasteboard for the specified representation type.

