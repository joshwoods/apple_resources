

- AppKit
- NSDocumentController
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

An object containing the error to present.

## Return Value

Returns true if error recovery was done; otherwise, false.

## Discussion

This method does not return until the user dismisses the alert and, if the error has recovery options and a recovery delegate, the error’s recovery delegate is sent an `attemptRecoveryFromError:optionIndex:` message.

The default `NSDocumentController` implementation of this method is equivalent to that of `NSResponder` while treating the application object as the next responder and forwarding error presentation messages to it. (The default `NSDocument` implementation of this method treats the shared `NSDocumentController` instance as the next responder and forwards these messages to it.) The default implementations of several `NSDocumentController` methods call this method.

The default implementation of this method calls willPresentError(_:) to give subclasses an opportunity to customize error presentation. You should not override this method but should instead override willPresentError(_:).

## See Also

### Handling Errors

func presentError(any Error, modalFor: NSWindow, delegate: Any?, didPresent: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents an error alert to the user as a modal panel.

func willPresentError(any Error) -> any Error

Indicates an error condition and provides the opportunity to return the same or a different error.

