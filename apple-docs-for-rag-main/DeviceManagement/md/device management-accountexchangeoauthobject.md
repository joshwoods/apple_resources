

- Device Management
-  AccountExchangeOAuthObject 

Object

# AccountExchangeOAuthObject

The declaration for configuring OAuth authentication of an Exchange account.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountExchangeOAuthObject
```

## Properties

`Enabled`

`boolean`

 (Required) 

If `true`, enables OAuth for this account.

`SignInURL`

`string`

The URL that this account uses for signing in with OAuth. The system ignores this value unless `Enabled` is `true`. The system doesn’t use autodiscovery when a declaraction contains this URL, so the declaration must also contain a `HostName`.

`TokenRequestURL`

`string`

The URL that this account uses for token requests with OAuth. The system ignores this value unless `Enabled` is `true`.

## See Also

### Supporting Objects

object AccountExchangeSMIMEObject

Settings for S/MIME.

object AccountExchangeSMIME_EncryptionObject

Settings for S/MIME encryption.

object AccountExchangeSMIME_SigningObject

Settings for S/MIME signing.

