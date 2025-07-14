

- Foundation
- NSExtensionContext
-  cancelRequest(withError:) 

Instance Method

# cancelRequest(withError:)

Tells the host app to cancel the app extension request, with a supplied error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancelRequest(withError error: any Error)
```

## Parameters 

`error`  

The error object to return. It must be non-`nil`.

## Discussion

On return, the `userInfo` dictionary of the NSError object contains a key named NSExtensionItemsAndErrorsKey which has as its value a dictionary of NSExtensionItem objects and associated NSError instances.

## See Also

### Related Documentation

App Extension Programming Guide

### Handling requests

func completeRequest(returningItems: [Any]?, completionHandler: ((Bool) -> Void)?)

Tells the host app to complete the app extension request with an array of result items.

let NSExtensionItemsAndErrorsKey: String

The extension items and errors key.

