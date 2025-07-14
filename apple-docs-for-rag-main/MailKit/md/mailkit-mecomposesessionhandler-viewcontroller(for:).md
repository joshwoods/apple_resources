

- MailKit
- MEComposeSessionHandler
-  viewController(for:) 

Instance Method

# viewController(for:)

Provides a custom view controller to display as part of the compose window.

macOS 12.0+

``` source
@MainActor
func viewController(for session: MEComposeSession) -> MEExtensionViewController
```

**Required**

## Parameters 

`session`  

The session that represents the properties of the message in the compose window.

## Return Value

A custom MEExtensionViewController subclass that Mail displays in the compose window.

## Discussion

To configure an icon and tooltip for the compose session handler’s view controller, add the following entries to your extension’s `Info.plist` file:

```
```

Include an icon in your extension’s bundle using the name you specify for MEComposeIcon.

Tip

Include the icon in an asset catalog in your extension’s bundle, and include both light and dark variants.

