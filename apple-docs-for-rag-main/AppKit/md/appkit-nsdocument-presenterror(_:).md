

- AppKit
- NSDocument
-  presentError(\_:) 

Instance Method

# presentError(\_:)

Presents an error alert to the user as a modal panel.

macOS

``` source
@MainActor
func presentError(_ error: any Error) -> Bool
```

## Parameters 

`error`  

The error object encapsulating the information to present to the user.

## Return Value

true if error recovery was done; otherwise, false.

## Discussion

This method does not return until the user dismisses the alert and, if the error has recovery options and a recovery delegate, the error’s recovery delegate is sent an attemptRecovery(fromError:optionIndex:) message.

The `NSDocument` default implementation of this method is equivalent to that of `NSResponder` and treats the shared `NSDocumentController` as the next responder and forwards these messages to it.

The default implementation of this method invokes willPresentError(_:) to give subclasses an opportunity to customize error presentation. You should not override this method but should instead override willPresentError(_:).

## See Also

### Displaying Errors to the User

func presentError(any Error, modalFor: NSWindow, delegate: Any?, didPresent: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents an error alert to the user as a modal panel.

func willPresentError(any Error) -> any Error

Called when the receiver is about to present an error.

func willNotPresentError(any Error)

Confirms that the error object is not to be presented to the user and the error cannot be recovered from, so cleanup can be done.

