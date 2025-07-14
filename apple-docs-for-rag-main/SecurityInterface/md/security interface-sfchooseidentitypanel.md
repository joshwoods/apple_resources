

- Security Interface
-  SFChooseIdentityPanel 

Class

# SFChooseIdentityPanel

A panel or sheet containing a list of identities that a user can choose from.

macOS 10.3+

``` source
@MainActor
class SFChooseIdentityPanel
```

## Overview

An identity is a digital certificate together with its associated private key. This class also allows the user to display the contents of any certificate in the list.

The following figure shows an example of a choose identity panel.

## Topics

### Returning a Shared Certificate Panel Object

class func shared() -> SFChooseIdentityPanel!

Returns a fully initialized, singleton choose identity panel object.

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

func informativeText() -> String!

Returns the informative text currently displayed in the panel.

func setInformativeText(String!)

Sets the optional informative text displayed in the panel.

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, identities: [Any]!, message: String!)

Displays a list of identities in a modal sheet from which the user can select an identity.

func runModal(forIdentities: [Any]!, message: String!) -> Int

Displays a list of identities in a modal panel.

### Getting Identity Information from a Sheet or Panel

func identity() -> Unmanaged&lt;SecIdentity>!

Returns the identity that the user chose in the panel or sheet.

### Working with Domains

func domain() -> String!

Returns the domain that will be associated with the chosen identity.

func setDomain(String!)

Sets an optional domain in which the identity is to be used.

### Delegate methods for providing help

func chooseIdentityPanelShowHelp(_ sender: SFChooseIdentityPanel!) -> Bool

Implements custom help behavior for the modal panel.

## Relationships

### Inherits From

- NSPanel

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

class SFCertificateTrustPanel

A panel or sheet that lets the user edit the trust settings in any of the certificates in a certificate chain.

class SFCertificateView

A view that displays the contents of a certificate, with options to display certificate details, display trust settings, and allow users to edit a certificate’s trust settings.

class SFChooseIdentityTableCellView

class SFKeychainSavePanel

A panel or sheet that allows the user to create a keychain.

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

