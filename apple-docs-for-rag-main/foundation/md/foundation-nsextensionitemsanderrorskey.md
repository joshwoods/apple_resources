

- Foundation
-  NSExtensionItemsAndErrorsKey 

Global Variable

# NSExtensionItemsAndErrorsKey

The extension items and errors key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSExtensionItemsAndErrorsKey: String
```

## Discussion

This key appears in the userInfo dictionary of the NSError object that cancelRequest(withError:) returns.

This key’s value is a dictionary of NSExtensionItem objects and associated NSError instances.

## See Also

### Handling requests

func completeRequest(returningItems: [Any]?, completionHandler: ((Bool) -> Void)?)

Tells the host app to complete the app extension request with an array of result items.

func cancelRequest(withError: any Error)

Tells the host app to cancel the app extension request, with a supplied error.

