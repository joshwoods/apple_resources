

- Collaboration
- CBIdentityPicker
-  runModal(for:modalDelegate:didEnd:contextInfo:) Deprecated

Instance Method

# runModal(for:modalDelegate:didEnd:contextInfo:)

Runs the receiver modally as a sheet attached to a specified window.

macOS 10.5–10.11Deprecated

``` source
func runModal(
    for window: NSWindow,
    modalDelegate delegate: Any?,
    didEnd didEndSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

Deprecated

Use runModal(for:completionHandler:) instead.

## Parameters 

`window`  

The parent window for the sheet.

`delegate`  

The delegate for the modal session.

`didEndSelector`  

A message sent to the delegate after the user responds but before the sheet is dismissed.

`contextInfo`  

Contextual data passed to the delegate in the `didEndSelector` message.

## Discussion

The `didEndSelector` parameter is a selector that takes three arguments. The corresponding method should have a declaration modeled on the following example:

```
```

where the `identityPicker` argument is the identity picker object, the `returnCode` argument is the button the user clicked, and `contextInfo` is the same `contextInfo` argument that was passed in the original message.

## See Also

### Related Documentation

Identity Services Programming Guide

### Running an Identity Picker

func runModal(for: NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Runs the identity picker modally as a sheet attached to a specified window.

func runModal() -> Int

Runs the receiver as an application-modal dialog.

