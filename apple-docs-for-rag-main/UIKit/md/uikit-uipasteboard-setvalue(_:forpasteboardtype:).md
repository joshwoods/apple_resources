

- UIKit
- UIPasteboard
-  setValue(\_:forPasteboardType:) 

Instance Method

# setValue(\_:forPasteboardType:)

Puts an object on the pasteboard for the specified representation type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setValue(
    _ value: Any,
    forPasteboardType pasteboardType: String
)
```

## Parameters 

`value`  

The object to be written to the pasteboard.

`pasteboardType`  

A string identifying the representation type of the pasteboard item. If the type is a UTI, it must be compatible with the class of `value`; otherwise, nothing is written to the pasteboard.

## Discussion

Use this method to put an object—such as an NSString, NSArray, NSDictionary, NSDate, NSNumber, UIImage, or NSURL object—on the pasteboard. (For images, you can also use the image or images properties; for all other data, such as raw binary data, use the setData(_:forPasteboardType:) method.) This method writes the object as the first item in the pasteboard. Calling this method replaces any items currently in the pasteboard.

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

func setData(Data, forPasteboardType: String)

Puts data on the pasteboard for the specified representation type.

func value(forPasteboardType: String) -> Any?

Returns an object on the pasteboard for the given representation type.

func values(forPasteboardType: String, inItemSet: IndexSet?) -> [Any]?

Returns the objects on the indicated pasteboard items that have the given representation type.

