

- Security Interface
- SFCertificatePanel
-  runModal(for:showGroup:) 

Instance Method

# runModal(for:showGroup:)

Displays a certificate chain in a modal panel.

macOS 10.4+

``` source
@MainActor
func runModal(
    for trust: SecTrust!,
    showGroup: Bool
) -> Int
```

## Parameters 

`trust`  

A SecTrust object associated with the certificate chain to display.

`showGroup`  

Specifies whether additional certificates (other than the leaf certificate) are displayed. To show only a single certificate, specify only one SecCertificate in the array and set `showGroup` to false.

## Return Value

This method returns the integer constant NSOKButton when dismissed.

## See Also

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, certificates: [Any]!, showGroup: Bool)

Displays one or more certificates in a modal sheet.

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, trust: SecTrust!, showGroup: Bool)

Displays a certificate chain in a modal sheet.

func certificateView() -> SFCertificateView!

Returns the certificate view for the modal panel.

func runModal(forCertificates: [Any]!, showGroup: Bool) -> Int

Displays one or more specified certificates in a modal panel.

