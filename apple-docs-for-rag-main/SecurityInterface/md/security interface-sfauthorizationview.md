

- Security Interface
-  SFAuthorizationView 

Class

# SFAuthorizationView

The class responsible for displaying a lock icon that can be used to indicate that a user interface has restricted access.

macOS 10.3+

``` source
@MainActor
class SFAuthorizationView
```

## Overview

The lock appears locked when the user must be authorized and appears open when the user has been authorized. The closed and open lock icons of the authorization view are shown in the following figure.

When you add an authorization view as a custom view to a window or dialog box, you must initialize it before it displays correctly. To initialize the view, use the setString(_:) method to create a default rights structure (containing a prompt string) or the setAuthorizationRights(_:) method to specify a rights structure. You must also either specify automatic updates (setAutoupdate(_:) or setAutoupdate(_:interval:)) or perform a manual update (updateStatus(_:)) to set the lock icon to its initial state.

You can implement delegate methods that are invoked when the authorization view changes state. You can optionally implement the delegate methods to obtain the state of the authorization object when you are using an authorization view.

When the user clicks a locked authorization view icon, the Security Server displays an authentication dialog (to request a user name and password, for example). When the user provides the requested credentials, the lock icon unlocks and the user is considered preauthorized to perform the functions specified by the authorization rights structure. You can call the updateStatus(_:) method to determine whether the user has been preauthorized: this method returns true if the view is in the unlocked state, otherwise false. Before committing changes or performing actions that require authorization, you should check the user’s authorization again, even if they are preauthorized.

The default behavior of this view is to preauthorize rights; if this is not possible it unlocks and waits for authorization to be checked when explicitly required.

## Topics

### Setting up the authorization view

func setString(AuthorizationString!)

Sets the requested-right string to use with the default authorization rights set.

func setAuthorizationRights(UnsafePointer&lt;AuthorizationRights>!)

Sets the authorization rights for this view.

func setAutoupdate(Bool)

Sets the authorization view to update itself automatically.

func setAutoupdate(Bool, interval: TimeInterval)

Sets the authorization view to update itself at a specific interval.

func setFlags(AuthorizationFlags)

Sets the current authorization flags for the view.

func setEnabled(Bool)

Sets the current state of the authorization view.

### Setting and getting the delegate for the view

func setDelegate(Any!)

Sets the delegate for this authorization view.

func delegate() -> Any!

Returns the delegate for this view.

### Updating the view

func updateStatus(Any!) -> Bool

Manually updates the authorization view.

### Getting information about the authorization view

func authorization() -> SFAuthorization!

Returns the authorization object associated with this view.

func authorizationRights() -> UnsafeMutablePointer&lt;AuthorizationRights>!

Returns the authorization rights for this view.

func authorizationState() -> SFAuthorizationViewState

Returns the current state of the authorization view.

func isEnabled() -> Bool

Indicates whether the authorization view is enabled (true) or disabled (false).

### Setting the authorization state

func authorize(Any!) -> Bool

Attempts to unlock the lock icon in the view.

func deauthorize(Any!) -> Bool

Sets the authorization state to unauthorized and locks the lock icon in the view.

### Delegate methods

func authorizationViewShouldDeauthorize(_ view: SFAuthorizationView!) -> Bool

Sent to the delegate when a user clicks the open lock icon.

func authorizationViewCreatedAuthorization(_ view: SFAuthorizationView!)

Sent to the delegate to indicate the authorization object has been created or changed.

func authorizationViewDidAuthorize(_ view: SFAuthorizationView!)

Sent to the delegate to indicate the user was authorized and the authorization view was changed to unlocked.

func authorizationViewDidDeauthorize(_ view: SFAuthorizationView!)

Sent to the delegate to indicate the user was deauthorized and the authorization view was changed to locked.

func authorizationViewDidHide(_ view: SFAuthorizationView!)

Sent to the delegate to indicate that the view’s visibility has changed.

func authorizationViewReleasedAuthorization(_ view: SFAuthorizationView!)

Sent to the delegate to indicate that deauthorization is about to occur.

### Constants

struct SFAuthorizationViewState

Defines the current state of the authorization view.

## Relationships

### Inherits From

- NSView

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

## See Also

### Classes

class SFAuthorizationPluginView

Allows authorization plug-in developers to create a custom view their plug-in can display.

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

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

