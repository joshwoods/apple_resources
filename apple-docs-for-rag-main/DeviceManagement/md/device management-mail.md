

- Device Management
-  Mail 

Device Management Profile

# Mail

The payload you use to configure a mail account on the device.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object Mail
```

## Properties

`allowMailDrop`

`boolean`

If `true`, the system enables this account to use Mail Drop.

Default: `false`

`disableMailRecentsSyncing`

`boolean`

If `true`, the system excludes this account from Recent Addresses syncing.

Default: `false`

`EmailAccountDescription`

`string`

A user-visible description of the email account, shown in the Mail and Settings applications.

`EmailAccountName`

`string`

The full user name for the account. The system displays this name in sent messages.

`EmailAccountType`

`string`

 (Required) 

Defines the protocol to use for the account.

Possible Values: `EmailTypeIMAP, EmailTypePOP`

`EmailAddress`

`string`

The full email address for the account. If this string isn’t present in the payload, the device prompts the user for this string during interactive profile installation in Settings or System Preferences.

`IncomingMailServerAuthentication`

`string`

 (Required) 

The authentication scheme for incoming mail.

Possible Values: `EmailAuthNone, EmailAuthPassword, EmailAuthCRAMMD5, EmailAuthNTLM, EmailAuthHTTPMD5`

`IncomingMailServerHostName`

`string`

 (Required) 

The incoming mail server host name.

`IncomingMailServerIMAPPathPrefix`

`string`

The path prefix for the IMAP mail server.

`IncomingMailServerPortNumber`

`integer`

The incoming mail server port number. If not set, the system uses the default port for a given protocol.

`IncomingMailServerUsername`

`string`

The user name for the email account, usually the same as the email address up to the “@” character. If not set and the account requires authentication for incoming email, the device prompts the user for this string during interactive profile installation in Settings or System Preferences.

`IncomingMailServerUseSSL`

`boolean`

If `true`, the system enables SSL for authentication on the incoming mail server.

Default: `false`

`IncomingPassword`

`string`

The password for the incoming mail server. The system only uses this password with encrypted profiles.

`OutgoingMailServerAuthentication`

`string`

 (Required) 

The authentication scheme for outgoing mail.

Possible Values: `EmailAuthNone, EmailAuthPassword, EmailAuthCRAMMD5, EmailAuthNTLM, EmailAuthHTTPMD5`

`OutgoingMailServerHostName`

`string`

 (Required) 

The outgoing mail server host name.

`OutgoingMailServerPortNumber`

`integer`

The outgoing mail server port number. If not set, the system uses ports 25, 587, and 465, in that order.

`OutgoingMailServerUsername`

`string`

The user name for the email account, usually the same as the email address up to the “@” character. If not set and the account requires authentication for outgoing email, the device prompts the user for this string during interactive profile installation in Settings or System Preferences.

`OutgoingMailServerUseSSL`

`boolean`

If `true`, the system enables SSL authentication on the outgoing mail server.

Default: `false`

`OutgoingPassword`

`string`

The password for the outgoing mail server. The system only uses this password with encrypted profiles.

`OutgoingPasswordSameAsIncomingPassword`

`boolean`

If `true`, the system prompts the user only once for the password, which it uses for both outgoing and incoming mail.

This setting is only supported by interactive profile installations. Not supported by non-interactive installations, such as MDM on iOS.

Default: `false`

`PreventAppSheet`

`boolean`

If `true`, the system prevents this account from sending mail in any app other than the Apple Mail app.

Default: `false`

`PreventMove`

`boolean`

If `true`, the system prevents moving messages out of this email account and into another account. It also prevents forwarding or replying from an account other than the recipient of the message.

Default: `false`

`SMIMEEnabled`

`boolean`

If `true`, the system enables S/MIME encryption. The system ignores this key in iOS 10.0 and later.

Default: `false`

`SMIMEEnableEncryptionPerMessageSwitch`

`boolean`

If `true`, the system displays the per-message encryption switch in the Mail Compose UI.

Default: `false`

`SMIMEEnablePerMessageSwitch`

`boolean`

Deprecated 

If `true`, the system displays the per-message encryption switch in the Mail Compose UI. Deprecated in iOS 12.0. Use `SMIMEEnableEncryptionPerMessageSwitch` instead.

Default: `false`

`SMIMEEncryptByDefault`

`boolean`

If `true`, the system enables S/MIME encryption by default.

Default: `false`

`SMIMEEncryptByDefaultUserOverrideable`

`boolean`

If `true`, the user can turn encryption by default on/off, and encryption is on.

Default: `false`

`SMIMEEncryptionCertificateUUID`

`string`

The UUID of the identity certificate used to decrypt messages sent to this account. The system attaches the public certificate to outgoing mail to allow the user to receive encrypted mail. When the user sends encrypted mail, the system uses the public certificate to encrypt the copy of the mail in their Sent mailbox.

`SMIMEEncryptionCertificateUUIDUserOverrideable`

`boolean`

If `true`, the user can select the S/MIME encryption identity, and encryption is on.

Default: `false`

`SMIMEEncryptionEnabled`

`boolean`

If `true`, the system enables S/MIME encryption for this account.

Default: `false`

`SMIMESigningCertificateUUID`

`string`

The payload UUID of the identity certificate used to sign messages sent from this account.

`SMIMESigningCertificateUUIDUserOverrideable`

`boolean`

If `true`, the user can select the signing identity.

Default: `false`

`SMIMESigningEnabled`

`boolean`

If `true`, the system enables S/MIME signing for this account.

Default: `false`

`SMIMESigningUserOverrideable`

`boolean`

If `true`, the user can turn S/MIME signing on or off in Settings.

Default: `false`

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.mail.managed` as the payload type.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS                     |
| User Channel               | macOS, Shared iPad      |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | iOS, macOS              |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad |

### Profile Example

```

    PayloadContent

            EmailAccountDescription
            Company Mail Account
            EmailAccountName
            Juan Chavez
            EmailAccountType
            EmailTypeIMAP
            EmailAddress
            juanchavez4@example.com
            IncomingMailServerAuthentication
            EmailAuthPassword
            IncomingMailServerHostName
            imap.example.com
            IncomingMailServerPortNumber
            993
            IncomingMailServerUseSSL

            IncomingMailServerUsername
            juanchavez4@example.com
            IncomingPassword
            Password123
            OutgoingMailServerAuthentication
            EmailAuthPassword
            OutgoingMailServerHostName
            smtp.example.com
            OutgoingMailServerPortNumber
            587
            OutgoingMailServerUseSSL

            OutgoingMailServerUsername
            juanchavez4@example.com
            OutgoingPassword
            Password123
            OutgoingPasswordSameAsIncomingPassword

            SMIMEEnablePerMessageSwitch

            SMIMEEnabled

            SMIMEEncryptionEnabled

            SMIMESigningEnabled

            allowMailDrop

            disableMailRecentsSyncing

            PayloadIdentifier
            com.example.mymailpayload
            PayloadType
            com.apple.mail.managed
            PayloadUUID
            d6379d8d-9e05-4d99-80bc-0865f1fe0aca
            PayloadVersion
            1

    PayloadDisplayName
    Mail
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    8e1961d8-898e-4d79-986f-c7a61af4103c
    PayloadVersion
    1

```

## See Also

### Mail

object ExchangeActiveSync

The payload you use to configure Exchange ActiveSync accounts.

object ExchangeWebServices

The payload you use to configure an Exchange Web Services account for Contacts, Mail, Notes, Reminders, and Calendar.

