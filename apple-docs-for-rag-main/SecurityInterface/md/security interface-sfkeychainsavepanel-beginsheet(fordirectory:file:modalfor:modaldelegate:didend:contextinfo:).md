

- Security Interface
- SFKeychainSavePanel
-  beginSheet(forDirectory:file:modalFor:modalDelegate:didEnd:contextInfo:) 

Instance Method

# beginSheet(forDirectory:file:modalFor:modalDelegate:didEnd:contextInfo:)

Displays a sheet that allows a user to create a new keychain.

macOS 10.3+

``` source
@MainActor
func beginSheet(
    forDirectory path: String!,
    file name: String!,
    modalFor docWindow: NSWindow!,
    modalDelegate delegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!
)
```

## Parameters 

`path`  

The path to the folder where the keychain is created. Specify `nil` for `~/Library/Keychains`.

`name`  

The keychain name to be automatically displayed in the Save As field of the sheet.

`docWindow`  

The parent window to which the sheet is attached. If this parameter is `nil`, the behavior defaults to a standalone modal window.

`delegate`  

The delegate object in which the method specified in the `didEndSelector` parameter is implemented.

`didEndSelector`  

A method selector for a delegate method called after the modal session has ended, but before the sheet has been dismissed. Implementation of this delegate method is optional.

`contextInfo`  

A pointer to data that is passed to the delegate method. You can use this data pointer for any purpose you wish.

## Discussion

The delegate method has the following signature:

```
- (void)createPanelDidEnd:(NSWindow *)sheet
        returnCode:(int)returnCode
        contextInfo:(void *)contextInfo
```

The parameters for the delegate method are:

`sheet`  
The window to which the sheet was attached.

`returnCode`  
The result code indicating which button the user clicked: either NSFileHandlingPanelOKButton or NSFileHandlingPanelCancelButton.

`contextInfo`  
Client-defined contextual data that is passed in the `contextInfo` parameter of the beginSheet(forDirectory:file:modalFor:modalDelegate:didEnd:contextInfo:) method.

The delegate method may dismiss the keychain settings sheet itself; if it does not, the sheet is dismissed on return from the `beginSheetForDirectory:...` method.

Use the keychain() method to obtain the keychain created by the user.

## Topics

### Related Documentation

func keychain() -> Unmanaged&lt;SecKeychain>!

Returns the keychain created by the keychain save panel.

func runModal(forDirectory: String!, file: String!) -> Int

Displays a panel that allows a user to create a new keychain.

## See Also

### Displaying a Sheet or Panel

func setPassword(String!)

Specifies the password for the keychain that will be created.

func runModal(forDirectory: String!, file: String!) -> Int

Displays a panel that allows a user to create a new keychain.

