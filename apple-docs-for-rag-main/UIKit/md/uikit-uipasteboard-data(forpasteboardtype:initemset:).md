

- UIKit
- UIPasteboard
-  data(forPasteboardType:inItemSet:) 

Instance Method

# data(forPasteboardType:inItemSet:)

Returns the data objects in the indicated pasteboard items that have the given representation type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func data(
    forPasteboardType pasteboardType: String,
    inItemSet itemSet: IndexSet?
) -> [Data]?
```

## Parameters 

`pasteboardType`  

A string identifying a representation type. Typically this is a UTI.

`itemSet`  

An index set with each integer value identifying a pasteboard item positionally in the pasteboard. Pass in `nil` to request all pasteboard items.

## Return Value

An array of NSData objects or, if a requested pasteboard item has no data of the the type indicated by `pasteboardType`, a NSNull object.

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

func data(forPasteboardType: String) -> Data?

Returns the data on the pasteboard for the given representation type.

func setData(Data, forPasteboardType: String)

Puts data on the pasteboard for the specified representation type.

func value(forPasteboardType: String) -> Any?

Returns an object on the pasteboard for the given representation type.

func values(forPasteboardType: String, inItemSet: IndexSet?) -> [Any]?

Returns the objects on the indicated pasteboard items that have the given representation type.

func setValue(Any, forPasteboardType: String)

Puts an object on the pasteboard for the specified representation type.

