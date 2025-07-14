

- AppKit
- NSDocument
-  willNotPresentError(\_:) 

Instance Method

# willNotPresentError(\_:)

Confirms that the error object is not to be presented to the user and the error cannot be recovered from, so cleanup can be done.

macOS 10.7+

``` source
@MainActor
func willNotPresentError(_ error: any Error)
```

## Parameters 

`error`  

An NSError object returned by another `NSDocument` method.

## Discussion

Some `NSDocument` methods, like those involved in writing, may not immediately delete temporary files if there is a chance that the error can be recovered from and the operation can continue. To make sure that cleanup is always done, you should invoke this method with `NSDocument` errors that are not going to be passed to one of the `presentError:...` methods. For example, the `NSDocument` implementation of the `NSFilePresenter` method savePresentedItemChanges(completionHandler:) invokes this method when it invokes autosave(withImplicitCancellability:completionHandler:) and the completion handler is passed an `NSError` object, because it does not present the error to the user.

## See Also

### Displaying Errors to the User

func presentError(any Error, modalFor: NSWindow, delegate: Any?, didPresent: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents an error alert to the user as a modal panel.

func presentError(any Error) -> Bool

Presents an error alert to the user as a modal panel.

func willPresentError(any Error) -> any Error

Called when the receiver is about to present an error.

