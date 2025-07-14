

- Security Interface
- SFCertificatePanel
-  beginSheet(for:modalDelegate:didEnd:contextInfo:certificates:showGroup:) 

Instance Method

# beginSheet(for:modalDelegate:didEnd:contextInfo:certificates:showGroup:)

Displays one or more certificates in a modal sheet.

macOS 10.3+

``` source
@MainActor
func beginSheet(
    for docWindow: NSWindow!,
    modalDelegate delegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!,
    certificates: [Any]!,
    showGroup: Bool
)
```

## Parameters 

`docWindow`  

The parent window to which the sheet is attached.

`delegate`  

The delegate object in which the method specified in the `didEndSelector` parameter is implemented.

`didEndSelector`  

A selector for a delegate method called when the sheet has been dismissed. Implementation of this delegate method is optional.

`contextInfo`  

A pointer to data that is passed to the delegate method. You can use this data pointer for any purpose you wish.

`certificates`  

The certificates to display. Pass an NSArray containing one or more objects of type SecCertificate in this parameter. The first certificate in the array must be the leaf certificate. The other certificates (if any) can be included in any order.

`showGroup`  

Specifies whether additional certificates (other than the leaf certificate) are displayed.

## Discussion

The behavior of this method is somewhat different in macOS 10.4 and later versus OS X v10.3. In OS X v10.3, the sheet displays whatever certificates you pass in the `certificates` parameter (provided the `showGroup` parameter is set to true). Starting with OS X v10.4, the sheet displays the leaf certificate (that is, the first certificate in the array you pass) plus any other certificates in the certificate chain that the Security Server can find. If you include all of the certificates in the chain in the `certificates` parameter, you can ensure that the same certificates are displayed whatever the version of the operating system, and may decrease the time required to find and display the certificates in macOS 10.4 and later.

The delegate method has the following signature:

```
```

The parameters for the delegate method are:

`sheet`  
The window to which the sheet was attached.

`returnCode`  
The result code indicating which button the user clicked: either NSFileHandlingPanelOKButton or NSFileHandlingPanelCancelButton.

`contextInfo`  
Client-defined contextual data that is passed in the `contextInfo` parameter of the `beginSheetForDirectory:...` method.

The delegate method may dismiss the keychain settings sheet itself; if it does not, the sheet is dismissed on return from the `beginSheetForDirectory:...` method.

## See Also

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, trust: SecTrust!, showGroup: Bool)

Displays a certificate chain in a modal sheet.

func certificateView() -> SFCertificateView!

Returns the certificate view for the modal panel.

func runModal(for: SecTrust!, showGroup: Bool) -> Int

Displays a certificate chain in a modal panel.

func runModal(forCertificates: [Any]!, showGroup: Bool) -> Int

Displays one or more specified certificates in a modal panel.

