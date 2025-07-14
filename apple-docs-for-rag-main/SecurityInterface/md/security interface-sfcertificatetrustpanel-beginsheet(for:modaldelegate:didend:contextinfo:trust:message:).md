

- Security Interface
- SFCertificateTrustPanel
-  beginSheet(for:modalDelegate:didEnd:contextInfo:trust:message:) 

Instance Method

# beginSheet(for:modalDelegate:didEnd:contextInfo:trust:message:)

Displays a modal sheet that shows the results of a certificate trust evaluation and that allows the user to edit trust settings.

macOS 10.3+

``` source
@MainActor
func beginSheet(
    for docWindow: NSWindow!,
    modalDelegate delegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!,
    trust: SecTrust!,
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

`trust`  

A trust management object. Use the SecTrustCreateWithCertificates(_:_:_:) function (in Security/SecTrust.h) to create the trust management object.

`message`  

A message string to display in the sheet.

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
Client-defined contextual data that is passed in the `contextInfo` parameter of the `beginSheetForWindow:...` method.

The delegate method may dismiss the keychain settings sheet itself; if it does not, the sheet is dismissed on return from the `beginSheetForWindow:...` method.

## Topics

### Related Documentation

func SecTrustCreateWithCertificates(_ certificates: CFTypeRef, _ policies: CFTypeRef?, _ trust: UnsafeMutablePointer&lt;SecTrust?>) -> OSStatus

Creates a trust management object based on certificates and policies.

func runModal(for: SecTrust!, message: String!) -> Int

Displays a modal panel that shows the results of a certificate trust evaluation and that allows the user to edit trust settings.

## See Also

### Displaying a Sheet or Panel

func runModal(for: SecTrust!, message: String!) -> Int

Displays a modal panel that shows the results of a certificate trust evaluation and that allows the user to edit trust settings.

