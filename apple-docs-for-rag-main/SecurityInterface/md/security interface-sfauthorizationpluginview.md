

- Security Interface
-  SFAuthorizationPluginView 

Class

# SFAuthorizationPluginView

Allows authorization plug-in developers to create a custom view their plug-in can display.

macOS 10.3+

``` source
class SFAuthorizationPluginView
```

## Overview

If you’re developing an authorization plug-in, you can subclass the SFAuthorizationPluginView class to create views that provide a custom user interface for your plug-in. By subclassing the SFAuthorizationPluginView class, you avoid changing or duplicating the Apple-provided authentication or login window dialogs to display your custom view.

To instantiate your SFAuthorizationPluginView subclass, you need the callbacks structure containing entry points to the Security Server that you receive in your plug-in’s AuthorizationPluginCreate function and the authorization engine handle you receive in your plug-in’s MechanismCreate function.

Your custom subclass of SFAuthorizationPluginView must override the following methods:

- buttonPressed(_:)

- view(for:)

## Topics

### Initializing an SFAuthorizationPluginView Object

init!(callbacks: UnsafePointer&lt;AuthorizationCallbacks>!, andEngineRef: AuthorizationEngineRef!)

Initializes a new authorization plug-in view with the specified callbacks and authorization engine handle.

### Getting Instance Information

func callbacks() -> UnsafePointer&lt;AuthorizationCallbacks>!

Returns the authorization callbacks structure with which this instance was initialized.

func engineRef() -> AuthorizationEngineRef!

Returns the authorization engine handle with which this instance was initialized.

func lastError() -> (any Error)!

Returns the last error that occurred during evaluation.

### Responding to User Actions

func buttonPressed(SFButtonType)

Tells the authorization plug-in that the user pressed a button in the custom view.

func view(for: SFViewType) -> NSView!

Returns the appropriate view object for the specified view type.

### Configuring the User Interface

func didActivate()

Tells the authorization plug-in when its user interface has become active.

func didDeactivate()

Tells the authorization plug-in that its user interface has been deactivated.

func willActivate(withUser: [AnyHashable : Any]!)

Tells the authorization plug-in that its user interface is about to be made active by the Apple-provided Security Agent.

### Setting Up the Keyboard Loop

func firstKeyView() -> NSView!

Returns the first view in the keyboard loop of the view.

func firstResponder() -> NSResponder!

Returns the view that should get focus for keyboard events.

func lastKeyView() -> NSView!

Returns the last view in the keyboard loop of the view.

### Enabling and Disabling Controls

func setEnabled(Bool)

Enables or disables the controls in the authorization plug-in’s view.

### Communicating with the Authorization Plug-in

func display()

Displays the user interface provided by the authorization plug-in view subclass.

func setButton(SFButtonType, enabled: Bool)

Enables or disables a button in the authorization plug-in’s user interface.

func update()

Tells the authorization plug-in to get and display the appropriate view in the authorization plug-in’s user interface.

### Constants

struct SFButtonType

These constants define the button types used by authorization plug-ins.

struct SFViewType

These constants define the view type requested by the authorization plug-in.

Exceptions

Exceptions thrown by the `SFAuthorizationPluginView` class

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

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

class SFKeychainSettingsPanel

A panel or sheet that allows users to change their keychain settings.

