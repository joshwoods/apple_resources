

- UIKit
- UIActivityItemSource
-  activityViewControllerPlaceholderItem(\_:) 

Instance Method

# activityViewControllerPlaceholderItem(\_:)

Returns the placeholder object for the data.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func activityViewControllerPlaceholderItem(_ activityViewController: UIActivityViewController) -> Any
```

**Required**

## Parameters 

`activityViewController`  

The activity view controller object requesting the placeholder item.

## Return Value

An object to use as a placeholder for the actual data.

## Discussion

This method returns an object that can be used as a placeholder for the real data. Placeholder objects don’t have to contain any real data but should be configured as closely as possible to the actual data object you intend to provide. In general the actual value should match in type but it’s possible to return a different type of data for activityViewController(_:itemForActivityType:). It should be one that the activity can handle otherwise you may get an activity with empty content. For example, the placeholder could be a UIImage object but the actual value could be an NSData object with PDF information.

## See Also

### Getting the data items

func activityViewController(UIActivityViewController, itemForActivityType: UIActivity.ActivityType?) -> Any?

Returns the data object to be acted upon.

**Required**

