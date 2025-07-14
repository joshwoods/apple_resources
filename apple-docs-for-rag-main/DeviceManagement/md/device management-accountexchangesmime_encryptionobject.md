

- Device Management
-  AccountExchangeSMIME_EncryptionObject 

Object

# AccountExchangeSMIME_EncryptionObject

Settings for S/MIME encryption.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountExchangeSMIME_EncryptionObject
```

## Properties

`Enabled`

`boolean`

 (Required) 

If `true`, the system enables S/MIME encryption by default, which the user can’t override if `PerMessageSwitchEnabled` is `false`.

`IdentityAssetReference`

`string`

Specifies the identifier of an asset declaration containing the identity required for S/MIME encryption. The system attaches the public certificate to outgoing mail to allow the user to receive encrypted mail. When the user sends encrypted mail, the system uses the public certificate to encrypt the copy of the mail in their Sent mailbox.

`IdentityUserOverrideable`

`boolean`

If `true`, the user can select an S/MIME signing identity in Settings.

Default: `false`

`PerMessageSwitchEnabled`

`boolean`

If `true`, the system enables the per-message encryption switch in the compose view.

Default: `false`

`UserOverrideable`

`boolean`

If `true`, the user can turn S/MIME encryption by default on or off in Settings.

Default: `false`

## See Also

### Supporting Objects

object AccountExchangeOAuthObject

The declaration for configuring OAuth authentication of an Exchange account.

object AccountExchangeSMIMEObject

Settings for S/MIME.

object AccountExchangeSMIME_SigningObject

Settings for S/MIME signing.

