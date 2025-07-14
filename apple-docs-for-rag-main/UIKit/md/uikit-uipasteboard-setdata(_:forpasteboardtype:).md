

- UIKit
- UIPasteboard
-  setData(\_:forPasteboardType:) 

Instance Method

# setData(\_:forPasteboardType:)

Puts data on the pasteboard for the specified representation type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setData(
    _ data: Data,
    forPasteboardType pasteboardType: String
)
```

## Parameters 

`data`  

The data object to be written to the pasteboard.

`pasteboardType`  

A string identifying the representation type of the pasteboard item. This is typically a UTI.

## Discussion

Use this method to put raw data on the pasteboard. For example, you could archive a graph of model objects and pass the resulting NSData object to a related app via a pasteboard using a custom pasteboard type. (To put objects—such as NSString, NSArray, NSDictionary, NSDate, NSNumber, UIImage, or NSURL objects—on the pasteboard, use the setValue(_:forPasteboardType:) method.) This method writes data for the first item in the pasteboard. Calling this method replaces any items currently in the pasteboard.

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

func data(forPasteboardType: String, inItemSet: IndexSet?) -> [Data]?

Returns the data objects in the indicated pasteboard items that have the given representation type.

func value(forPasteboardType: String) -> Any?

Returns an object on the pasteboard for the given representation type.

func values(forPasteboardType: String, inItemSet: IndexSet?) -> [Any]?

Returns the objects on the indicated pasteboard items that have the given representation type.

func setValue(Any, forPasteboardType: String)

Puts an object on the pasteboard for the specified representation type.

