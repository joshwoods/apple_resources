

- UIKit
- UIPasteboard
-  value(forPasteboardType:) 

Instance Method

# value(forPasteboardType:)

Returns an object on the pasteboard for the given representation type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func value(forPasteboardType pasteboardType: String) -> Any?
```

## Parameters 

`pasteboardType`  

A string identifying a representation type of a pasteboard item.

## Return Value

An object that is an instance of the appropriate class based on `pasteboardType` or an NSData object containing “raw” data.

## Discussion

This method attempts to return an object that is of a class type appropriate to the representation type, which typically is a UTI. For example, if the representation type is `kUTTypePlainText` (`public.plain-text`), the method returns an NSString object. If the method can’t determine the class type from the representation type, it returns the object as a generic object, such as an NSString, NSArray, NSDictionary, NSDate, NSNumber, NSURL, UIImage, or NSData object. This method works on the first item in the pasteboard. If there are other items, it ignores them.

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

func values(forPasteboardType: String, inItemSet: IndexSet?) -> [Any]?

Returns the objects on the indicated pasteboard items that have the given representation type.

func setValue(Any, forPasteboardType: String)

Puts an object on the pasteboard for the specified representation type.

