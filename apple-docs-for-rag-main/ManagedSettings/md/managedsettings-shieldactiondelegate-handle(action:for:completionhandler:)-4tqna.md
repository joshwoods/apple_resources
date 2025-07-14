

- ManagedSettings
- ShieldActionDelegate
-  handle(action:for:completionHandler:) 

Instance Method

# handle(action:for:completionHandler:)

Allows the extension to respond to a user action when the system displays a shield over a website.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func handle(
    action: ShieldAction,
    for webDomain: WebDomainToken,
    completionHandler: @escaping (ShieldActionResponse) -> Void
)
```

## Parameters 

`action`  

The user’s action.

`webDomain`  

The web domain that the shield covers.

`completionHandler`  

A closure for your extension to call after you handle the user’s action.

