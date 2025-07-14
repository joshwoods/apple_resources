

- Security Interface
- SFCertificatePanel
-  certificateView() 

Instance Method

# certificateView()

Returns the certificate view for the modal panel.

macOS 10.4+

``` source
@MainActor
func certificateView() -> SFCertificateView!
```

## See Also

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, certificates: [Any]!, showGroup: Bool)

Displays one or more certificates in a modal sheet.

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, trust: SecTrust!, showGroup: Bool)

Displays a certificate chain in a modal sheet.

func runModal(for: SecTrust!, showGroup: Bool) -> Int

Displays a certificate chain in a modal panel.

func runModal(forCertificates: [Any]!, showGroup: Bool) -> Int

Displays one or more specified certificates in a modal panel.

