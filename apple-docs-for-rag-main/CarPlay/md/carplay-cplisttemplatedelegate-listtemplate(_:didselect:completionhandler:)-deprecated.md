

- CarPlay
- CPListTemplateDelegate
-  listTemplate(\_:didSelect:completionHandler:) Deprecated

Instance Method

# listTemplate(\_:didSelect:completionHandler:)

Tells the delegate when the user selects a list item.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func listTemplate(
    _ listTemplate: CPListTemplate,
    didSelect item: CPListItem,
    completionHandler: @escaping () -> Void
)
```

``` source
func listTemplate(
    _ listTemplate: CPListTemplate,
    didSelect item: CPListItem
) async
```

**Required**

## Parameters 

`listTemplate`  

The list template that contains the selected item.

`item`  

The item that the user selects.

`completionHandler`  

The block that your app must call after handling the selected item.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When implementing this method, perform any necessary operations to prepare for completing the item selection, including updating your user interface. You must call `completionHandler` after handling the selected item to tell the system that it can continue. The list template displays an activity indicator—after a short delay—while it waits for your implementation to call the completion handler.

