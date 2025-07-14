

- Security Interface
- SFChooseIdentityPanel
-  beginSheet(for:modalDelegate:didEnd:contextInfo:identities:message:) 

Instance Method

# beginSheet(for:modalDelegate:didEnd:contextInfo:identities:message:)

Displays a list of identities in a modal sheet from which the user can select an identity.

macOS 10.3+

``` source
@MainActor
func beginSheet(
    for docWindow: NSWindow!,
    modalDelegate delegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!,
    identities: [Any]!,
    message: String!
)
```

## Parameters 

`docWindow`  

The parent window to which the sheet is attached.

`delegate`  

The delegate object in which the method specified in the `didEndSelector` parameter is implemented.

`didEndSelector`  

A method selector for a delegate method called when the sheet has been dismissed. Implementation of this delegate method is optional.

`contextInfo`  

A pointer to data that is passed to the delegate method. You can use this data pointer for any purpose you wish.

`identities`  

An array of identity objects (objects of type SecIdentity). Use the SecIdentitySearchCopyNext function (in Security/SecIdentitySearch.h) to find identity objects.

`message`  

A message string to display in the sheet.

## Discussion

Use the `identity` method to obtain the identity chosen by the user.

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
Client-defined contextual data that is passed in the `contextInfo` parameter of the `beginSheetForWindow:...` method.

The sheet is dismissed on return from the `beginSheetForWindow:...` method.

## Topics

### Related Documentation

func runModal(forIdentities: [Any]!, message: String!) -> Int

Displays a list of identities in a modal panel.

func identity() -> Unmanaged&lt;SecIdentity>!

Returns the identity that the user chose in the panel or sheet.

## See Also

### Displaying a Sheet or Panel

func runModal(forIdentities: [Any]!, message: String!) -> Int

Displays a list of identities in a modal panel.

