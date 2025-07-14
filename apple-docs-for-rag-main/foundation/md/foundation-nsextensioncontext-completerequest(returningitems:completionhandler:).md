

- Foundation
- NSExtensionContext
-  completeRequest(returningItems:completionHandler:) 

Instance Method

# completeRequest(returningItems:completionHandler:)

Tells the host app to complete the app extension request with an array of result items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func completeRequest(
    returningItems items: [Any]?,
    completionHandler: ((Bool) -> Void)? = nil
)
```

## Parameters 

`items`  

An array of result items, each an NSExtensionItem object, to return to the host app.

`completionHandler`  

An optional block to be called when the request completes, performed as a background priority task.

The block takes the following parameter:

expired  
A Boolean value that indicates whether the system is terminating a previous invocation of the `completionHandler` block.

This parameter is true when the system prematurely terminates a `completionHandler` block that was previously invoked and had not otherwise expired.

Important

If the system calls your block with an `expired` value of true, you must immediately suspend your app extension. If you fail to do this, the system terminates your extension’s process.

When your app extension exits, all concurrent requests being handled by the extension, serving the same or other host apps, are terminated.

## Discussion

Calling this method eventually dismisses the app extension’s view controller.

## See Also

### Handling requests

func cancelRequest(withError: any Error)

Tells the host app to cancel the app extension request, with a supplied error.

let NSExtensionItemsAndErrorsKey: String

The extension items and errors key.

