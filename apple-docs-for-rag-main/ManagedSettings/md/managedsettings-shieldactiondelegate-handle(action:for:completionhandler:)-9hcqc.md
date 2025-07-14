

- ManagedSettings
- ShieldActionDelegate
-  handle(action:for:completionHandler:) 

Instance Method

# handle(action:for:completionHandler:)

Allows the extension to respond to a user action when the system displays a shield over an application or website because of its category.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func handle(
    action: ShieldAction,
    for category: ActivityCategoryToken,
    completionHandler: @escaping (ShieldActionResponse) -> Void
)
```

## Parameters 

`action`  

The user’s action.

`category`  

The category of the application or website that the shield covers.

`completionHandler`  

A closure for your extension to call after you handle the user’s action.

