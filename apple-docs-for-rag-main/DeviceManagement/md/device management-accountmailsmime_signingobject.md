

- Device Management
-  AccountMailSMIME_SigningObject 

Object

# AccountMailSMIME_SigningObject

Settings for S/MIME signing.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountMailSMIME_SigningObject
```

## Properties

`Enabled`

`boolean`

 (Required) 

If `true`, the system enables S/MIME signing.

`IdentityAssetReference`

`string`

Specifies the identifier of an asset declaration containing the identity required for S/MIME signing of messages sent from this account.

`IdentityUserOverrideable`

`boolean`

If `true`, the user can select an S/MIME signing identity in Settings.

Default: `false`

`UserOverrideable`

`boolean`

If `true`, the user can turn S/MIME signing on or off in Settings.

Default: `false`

## See Also

### Supporting Objects

object AccountMailIncomingServerObject

The settings for configuring an incoming mail server.

object AccountMailOutgoingServerObject

The settings for configuring an outgoing mail server.

object AccountMailSMIMEObject

Settings for S/MIME.

object AccountMailSMIME_EncryptionObject

Settings for S/MIME encryption.

