

- Security Interface
-  SFCertificateView 

Class

# SFCertificateView

A view that displays the contents of a certificate, with options to display certificate details, display trust settings, and allow users to edit a certificate’s trust settings.

macOS 10.3+

``` source
@MainActor
class SFCertificateView
```

## Overview

The following figure shows a certificate view that includes editable trust settings and certificate details.

## Topics

### Specifying the Certificate to Display

func setCertificate(SecCertificate!)

Specifies the certificate that’s displayed in the view.

### Customizing the Appearance and Behavior of the View

func setDetailsDisclosed(Bool)

Sets whether the certificate details subview is disclosed.

func setDisplayDetails(Bool)

Specifies whether the user can see the certificate details.

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

func setPolicies(Any!)

Specifies the policies to use when evaluating this certificate’s status.

func setPoliciesDisclosed(Bool)

Specifies whether the trust policy settings subview is disclosed.

### Getting Information About the View

func certificate() -> Unmanaged&lt;SecCertificate>!

Returns the certificate currently displayed in the view.

func detailsDisplayed() -> Bool

Indicates if the view currently shows the certificate’s details.

func detailsDisclosed() -> Bool

Returns whether the view currently shows the certificate’s details.

func isTrustDisplayed() -> Bool

Indicates if the view currently shows the certificate’s trust settings.

func isEditable() -> Bool

Indicates if the view allows the user to edit the certificate’s trust.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificate.

func policiesDisclosed() -> Bool

Returns whether the trust policy subview is disclosed.

### Saving User Trust Settings

func saveTrustSettings()

Saves the user’s current trust settings for the displayed certificate.

### Constants

Notifications

Notifications sent by this class.

## Relationships

### Inherits From

- NSVisualEffectView

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
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

class SFChooseIdentityPanel

A panel or sheet containing a list of identities that a user can choose from.

class SFChooseIdentityTableCellView

class SFKeychainSavePanel

A panel or sheet that allows the user to create a keychain.

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

