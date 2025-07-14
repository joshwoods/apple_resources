

- Collaboration
- CBIdentityPicker
-  runModal(for:completionHandler:) 

Instance Method

# runModal(for:completionHandler:)

Runs the identity picker modally as a sheet attached to a specified window.

macOS 10.5+

``` source
func runModal(
    for window: NSWindow,
    completionHandler: ((NSApplication.ModalResponse) -> Void)? = nil
)
```

``` source
func runModal(for window: NSWindow) async -> NSApplication.ModalResponse
```

## Parameters 

`window`  

The parent window for the sheet.

`completionHandler`  

The handler to run after the return value is known, but before the sheet is dismissed.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Running an Identity Picker

func runModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the receiver modally as a sheet attached to a specified window.

Deprecated

func runModal() -> Int

Runs the receiver as an application-modal dialog.

