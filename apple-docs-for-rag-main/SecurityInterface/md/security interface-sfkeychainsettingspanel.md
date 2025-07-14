

- Security Interface
-  SFKeychainSettingsPanel 

Class

# SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

macOS 10.3+

``` source
@MainActor
class SFKeychainSettingsPanel
```

## Overview

Keychain settings include:

- Lock after a set period of inactivity

- Lock on sleep

- Synchronize using .Mac

The following figure shows an example of a keychain settings panel.

For more information, see Keychain Services Programming Guide.

## Topics

### Returning a shared keychain save panel object

class func shared() -> SFKeychainSettingsPanel!

Returns a shared keychain settings panel object.

### Displaying a sheet or panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, settings: UnsafeMutablePointer&lt;SecKeychainSettings>!, keychain: SecKeychain!)

Displays a sheet that allows users to change keychain settings.

func runModal(for: UnsafeMutablePointer&lt;SecKeychainSettings>!, keychain: SecKeychain!) -> Int

Displays a panel that allows users to change keychain settings.

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

class SFChooseIdentityPanel

A panel or sheet containing a list of identities that a user can choose from.

class SFChooseIdentityTableCellView

class SFKeychainSavePanel

A panel or sheet that allows the user to create a keychain.

