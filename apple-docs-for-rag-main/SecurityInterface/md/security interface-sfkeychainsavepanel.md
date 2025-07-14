

- Security Interface
-  SFKeychainSavePanel 

Class

# SFKeychainSavePanel

A panel or sheet that allows the user to create a keychain.

macOS 10.3+

``` source
@MainActor
class SFKeychainSavePanel
```

## Overview

The following figure shows an example of a keychain save panel.

## Topics

### Returning a Shared Keychain Save Panel Object

class func shared() -> SFKeychainSavePanel!

Returns a shared keychain save panel object.

### Displaying a Sheet or Panel

func setPassword(String!)

Specifies the password for the keychain that will be created.

func beginSheet(forDirectory: String!, file: String!, modalFor: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays a sheet that allows a user to create a new keychain.

func runModal(forDirectory: String!, file: String!) -> Int

Displays a panel that allows a user to create a new keychain.

### Returning Information from the Sheet or Panel

func error() -> (any Error)!

Returns the last error encountered by the keychain save panel.

func keychain() -> Unmanaged&lt;SecKeychain>!

Returns the keychain created by the keychain save panel.

## Relationships

### Inherits From

- NSSavePanel

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

class SFChooseIdentityPanel

A panel or sheet containing a list of identities that a user can choose from.

class SFChooseIdentityTableCellView

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

