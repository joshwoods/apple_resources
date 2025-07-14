

- UIKit
- UIActivityItemSource
-  activityViewController(\_:itemForActivityType:) 

Instance Method

# activityViewController(\_:itemForActivityType:)

Returns the data object to be acted upon.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func activityViewController(
    _ activityViewController: UIActivityViewController,
    itemForActivityType activityType: UIActivity.ActivityType?
) -> Any?
```

**Required**

## Parameters 

`activityViewController`  

The activity view controller object requesting the data item.

`activityType`  

The type of activity to be performed with the data object. You can use this string to decide how best to prepare the data object.

## Return Value

The final data object to be acted on. May be `nil` if multiple items were registered for a single activity type, so long as one of the items returns an actual value.

## Discussion

This method returns the actual data object to be acted on by an activity object. Your implementation of this method should create or generate the data object and return it as quickly as possible.

## See Also

### Getting the data items

func activityViewControllerPlaceholderItem(UIActivityViewController) -> Any

Returns the placeholder object for the data.

**Required**

