

- AppKit
- NSDocumentController
-  presentError(\_:modalFor:delegate:didPresent:contextInfo:) 

Instance Method

# presentError(\_:modalFor:delegate:didPresent:contextInfo:)

Presents an error alert to the user as a modal panel.

macOS

``` source
@MainActor
func presentError(
    _ error: any Error,
    modalFor window: NSWindow,
    delegate: Any?,
    didPresent didPresentSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`error`  

The error to present.

`window`  

The window to present the error.

`delegate`  

The object to receive the selector.

`didPresentSelector`  

The selector to send to the delegate.

`contextInfo`  

A pointer to user-supplied data.

## Discussion

When the user dismisses the alert and any recovery possible for the error and chosen by the user has been attempted, sends the message `didPresentSelector` to the specified `delegate`. The method selected by `didPresentSelector` must have the same signature as:

```
- (void)didPresentErrorWithRecovery:(BOOL)didRecover contextInfo:(void  *)contextInfo;
```

The default `NSDocumentController` implementation of this method is equivalent to that of `NSResponder` while treating the application object as the next responder and forwarding error presentation messages to it. (The default `NSDocument` implementation of this method treats the shared `NSDocumentController` instance as the next responder and forwards these messages to it.)

The default implementation of this method calls willPresentError(_:) to give subclasses an opportunity to customize error presentation. You should not override this method but should instead override willPresentError(_:).

## See Also

### Handling Errors

func presentError(any Error) -> Bool

Presents an error alert to the user as a modal panel.

func willPresentError(any Error) -> any Error

Indicates an error condition and provides the opportunity to return the same or a different error.

