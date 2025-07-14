

- Device Management
-  AccountMailOutgoingServerObject 

Object

# AccountMailOutgoingServerObject

The settings for configuring an outgoing mail server.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountMailOutgoingServerObject
```

## Properties

`AuthenticationCredentialsAssetReference`

`string`

The identifier of an asset declaration that contains the credentials for this account to authenticate with an outgoing mail server. The corresponding asset must be of type `CredentialUserNameAndPassword`.

If the `AuthenticationMethod` is `None`, this field must be blank. Otherwise, the declaration must contain this field.

`AuthenticationMethod`

`string`

 (Required) 

The authentication method for the outgoing mail server.

Possible Values: `None, Password, CRAMMD5, NTLM, HTTPMD5`

`HostName`

`string`

 (Required) 

The host name for the outgoing mail server.

`Port`

`integer`

The port number for the outgoing mail server.

## See Also

### Supporting Objects

object AccountMailIncomingServerObject

The settings for configuring an incoming mail server.

object AccountMailSMIMEObject

Settings for S/MIME.

object AccountMailSMIME_EncryptionObject

Settings for S/MIME encryption.

object AccountMailSMIME_SigningObject

Settings for S/MIME signing.

