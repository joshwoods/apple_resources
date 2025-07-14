

- AppKit
- NSResponder
-  presentError(\_:) 

Instance Method

# presentError(\_:)

Presents an error alert to the user as an application-modal dialog.

macOS

``` source
@MainActor
func presentError(_ error: any Error) -> Bool
```

## Parameters 

`error`  

An object containing information about an error.

## Discussion

The alert displays information found in the NSError object `error`; this information can include error description, recovery suggestion, failure reason, and button titles (all localized). The method returns true if error recovery succeeded and false otherwise. For error recovery to be attempted, an recovery-attempter object (that is, an object conforming to the `NSErrorRecoveryAttempting` informal protocol) must be associated with `error`.

The default implementation of this method sends willPresentError(_:) to `self`. By doing this, `NSResponder` gives subclasses an opportunity to customize error presentation. It then forwards the message, passing any customized error object, to the next responder; if there is no next responder, it passes the error object to `NSApp`, which displays a document-modal error alert. When the user dismisses the alert, any recovery attempter associated with the error object is given a chance to recover from the error. See the class description for the precise route up the responder chain (plus document and controller objects) this message might travel.

It is not recommended that you attempt to override this method. If you wish to customize the error presentation, override willPresentError(_:) instead.

## See Also

### Presenting and Customizing Error Information

func presentError(any Error, modalFor: NSWindow, delegate: Any?, didPresent: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents an error alert to the user as a document-modal sheet attached to document window.

func willPresentError(any Error) -> any Error

Returns a custom version of the supplied error object that’s more suitable for presentation in alert sheets and dialogs.

