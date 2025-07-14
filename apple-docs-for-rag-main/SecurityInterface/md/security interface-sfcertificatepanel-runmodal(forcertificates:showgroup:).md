

- Security Interface
- SFCertificatePanel
-  runModal(forCertificates:showGroup:) 

Instance Method

# runModal(forCertificates:showGroup:)

Displays one or more specified certificates in a modal panel.

macOS 10.3+

``` source
@MainActor
func runModal(
    forCertificates certificates: [Any]!,
    showGroup: Bool
) -> Int
```

## Parameters 

`certificates`  

The certificates to display. Pass an NSArray containing one or more objects of type SecCertificate in this parameter. The first certificate in the array must be the leaf certificate. The other certificates (if any) can be included in any order.

`showGroup`  

Specifies whether additional certificates (other than the leaf certificate) are displayed. To show only a single certificate, specify only one SecCertificate in the array and set `showGroup` to false.

## Return Value

This method returns the integer constant NSOKButton when dismissed.

## Discussion

The behavior of this method is somewhat different in macOS 10.4 and later versus OS X v10.3. In OS X v10.3, the panel displays whatever certificates you pass in the `certificates` parameter (provided the `showGroup` parameter is set to true). Starting with OS X v10.4, the panel displays the leaf certificate (that is, the first certificate in the array you pass) plus any other certificates in the certificate chain that the Security Server can find. If you include all of the certificates in the chain in the `certificates` parameter, you can ensure that the same certificates are displayed whatever the version of the operating system, and may decrease the time required to find and display the certificates in macOS 10.4 and later.

## See Also

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, certificates: [Any]!, showGroup: Bool)

Displays one or more certificates in a modal sheet.

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, trust: SecTrust!, showGroup: Bool)

Displays a certificate chain in a modal sheet.

func certificateView() -> SFCertificateView!

Returns the certificate view for the modal panel.

func runModal(for: SecTrust!, showGroup: Bool) -> Int

Displays a certificate chain in a modal panel.

