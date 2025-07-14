

- Security Interface
-  SFCertificateTrustPanel 

Class

# SFCertificateTrustPanel

A panel or sheet that lets the user edit the trust settings in any of the certificates in a certificate chain.

macOS 10.3+

``` source
@MainActor
class SFCertificateTrustPanel
```

## Overview

The following figure shows an example of a certificate trust panel.

You can use this class to enable a user to make trust decisions when one or more certificates required for an operation are invalid or cannot be verified.

To display a certificate in a panel or sheet without editable trust settings, use the SFCertificatePanel class. To display certificates in a custom view, use the SFCertificateView class.

## Topics

### Returning a Shared Certificate Trust Panel Object

class func shared() -> SFCertificateTrustPanel!

Returns a fully initialized, singleton certificate trust panel object.

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, trust: SecTrust!, message: String!)

Displays a modal sheet that shows the results of a certificate trust evaluation and that allows the user to edit trust settings.

func runModal(for: SecTrust!, message: String!) -> Int

Displays a modal panel that shows the results of a certificate trust evaluation and that allows the user to edit trust settings.

### Controlling the Appearance of a Certificate Trust Panel

func informativeText() -> String!

Returns the (optional) informative text currently displayed in the panel.

func setInformativeText(String!)

Sets the (optional) informative text displayed in the panel.

## Relationships

### Inherits From

- SFCertificatePanel

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSMenuItemValidation
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable

## See Also

### Classes

class SFAuthorizationPluginView

Allows authorization plug-in developers to create a custom view their plug-in can display.

class SFAuthorizationView

The class responsible for displaying a lock icon that can be used to indicate that a user interface has restricted access.

class SFCertificatePanel

A panel or sheet that displays one or more certificates.

class SFCertificateView

A view that displays the contents of a certificate, with options to display certificate details, display trust settings, and allow users to edit a certificate’s trust settings.

class SFChooseIdentityPanel

A panel or sheet containing a list of identities that a user can choose from.

class SFChooseIdentityTableCellView

class SFKeychainSavePanel

A panel or sheet that allows the user to create a keychain.

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

