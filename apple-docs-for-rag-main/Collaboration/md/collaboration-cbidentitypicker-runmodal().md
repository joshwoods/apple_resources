

- Collaboration
- CBIdentityPicker
-  runModal() 

Instance Method

# runModal()

Runs the receiver as an application-modal dialog.

macOS 10.5+

``` source
func runModal() -> Int
```

## Return Value

`NSOKButton` if the user selected OK; otherwise, `NSCancelButton`.

## Discussion

The receiver may create identities for selected records if necessary.

## See Also

### Running an Identity Picker

func runModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the receiver modally as a sheet attached to a specified window.

Deprecated

func runModal(for: NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Runs the identity picker modally as a sheet attached to a specified window.

