

- UIKit
- UIPasteboard
-  setItems(\_:options:) 

Instance Method

# setItems(\_:options:)

Adds an array of items to a pasteboard, and sets privacy options for all the items on the pasteboard.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setItems(
    _ items: [[String : Any]],
    options: [UIPasteboard.OptionsKey : Any] = [:]
)
```

## Parameters 

`items`  

An array of items to add to the pasteboard.

`options`  

The privacy options to apply to all the items on the pasteboard. The available options are described in UIPasteboard.OptionsKey.

## See Also

### Getting and setting pasteboard items

var numberOfItems: Int

The number of items for the pasteboard.

var items: [[String : Any]]

The pasteboard items on the pasteboard.

func addItems([[String : Any]])

Appends pasteboard items to the current contents of the pasteboard.

func data(forPasteboardType: String) -> Data?

Returns the data on the pasteboard for the given representation type.

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

