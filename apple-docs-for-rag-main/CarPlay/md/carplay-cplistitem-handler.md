

- CarPlay
- CPListItem
-  handler 

Instance Property

# handler

An optional closure that CarPlay invokes when the user selects the list item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var handler: ((any CPSelectableListItem, @escaping () -> Void) -> Void)? { get set }
```

## Discussion

In Swift, the handler is a closure that has two parameters:

- An object that conforms to CPSelectableListItem, which is the list item that the user selects.

- The completion closure you call to notify CarPlay when you finish processing the selection.

In Objective-C, the block’s parameters are:

`item`  
The list item that the user selects.

`completionBlock`  
The block you call to notify CarPlay when you finish processing the selection.

CarPlay executes your handler on the main queue. You must call the completion closure, or `completionBlock` in Objective-C, after you finish processing the selection. If you need to perform asynchronous tasks, dispatch them to a background queue and call the completion closure or `completionBlock` when they complete. CarPlay displays an asynchronous progress indicator until you call the completion closure.

## See Also

### Managing Configuration

var isEnabled: Bool

A Boolean value that indicates if the item is enabled.

var userInfo: Any?

An opaque value for the list item.

