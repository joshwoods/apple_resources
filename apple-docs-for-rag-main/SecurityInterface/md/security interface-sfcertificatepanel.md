

- Security Interface
-  SFCertificatePanel 

Class

# SFCertificatePanel

A panel or sheet that displays one or more certificates.

macOS 10.3+

``` source
@MainActor
class SFCertificatePanel
```

## Overview

The following figure shows an example of a certificate panel.

An SFCertificatePanel can optionally display all of the certificates in a certificate chain.

This class displays certificate details, but not trust settings. To display a certificate with editable trust settings in a panel or sheet, use the SFCertificateTrustPanel class. To display certificates in a custom view, use the SFCertificateView class.

Note that for macOS 10.4 and later, this class displays the evaluation status for each certificate. You can modify how the certificates are evaluated by calling the setPolicies(_:) method.

## Topics

### Returning a Shared Certificate Panel Object

class func shared() -> SFCertificatePanel!

Returns a fully initialized, singleton certificate panel object.

### Providing Help

func setHelpAnchor(String!)

Sets the help anchor string for the sheet or modal panel.

func setShowsHelp(Bool)

Displays a Help button in the sheet or panel.

func helpAnchor() -> String!

Returns the current help anchor string for the sheet or panel.

func showsHelp() -> Bool

Indicates whether the help button is currently set to be displayed.

### Customizing the Appearance of the Sheet or Panel

func setAlternateButtonTitle(String!)

Customizes the title of the alternate button.

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func setPolicies(Any!)

Specifies one or more policies that apply to the displayed certificates.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificates.

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, certificates: [Any]!, showGroup: Bool)

Displays one or more certificates in a modal sheet.

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, trust: SecTrust!, showGroup: Bool)

Displays a certificate chain in a modal sheet.

func certificateView() -> SFCertificateView!

Returns the certificate view for the modal panel.

func runModal(for: SecTrust!, showGroup: Bool) -> Int

Displays a certificate chain in a modal panel.

func runModal(forCertificates: [Any]!, showGroup: Bool) -> Int

Displays one or more specified certificates in a modal panel.

### Delegate method for providing help

func certificatePanelShowHelp(_ sender: SFCertificatePanel!) -> Bool

Implements custom help behavior for the modal panel.

## Relationships

### Inherits From

- NSPanel

### Inherited By

- SFCertificateTrustPanel

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

class SFCertificateTrustPanel

A panel or sheet that lets the user edit the trust settings in any of the certificates in a certificate chain.

class SFCertificateView

A view that displays the contents of a certificate, with options to display certificate details, display trust settings, and allow users to edit a certificate’s trust settings.

class SFChooseIdentityPanel

A panel or sheet containing a list of identities that a user can choose from.

class SFChooseIdentityTableCellView

class SFKeychainSavePanel

A panel or sheet that allows the user to create a keychain.

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

