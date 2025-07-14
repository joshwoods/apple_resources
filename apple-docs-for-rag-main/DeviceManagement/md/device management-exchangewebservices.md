

- Device Management
-  ExchangeWebServices 

Device Management Profile

# ExchangeWebServices

The payload you use to configure an Exchange Web Services account for Contacts, Mail, Notes, Reminders, and Calendar.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ExchangeWebServices
```

## Properties

`allowMailDrop`

`boolean`

If `true`, the system enables Mail Drop.

Default: `false`

`AuthenticationCertificateUUID`

`string`

The UUID of the certificate payload within the same profile to use for the identity credential. Supported on macOS 10.11 or later. On macOS 10.12 or later use the PayloadCertificateUUID.

`EmailAddress`

`string`

The full email address for the account. If the email address string isn’t present in the payload, the device prompts for it during profile installation.

`ExternalHost`

`string`

The external server address.

`ExternalPath`

`string`

The external server path.

`ExternalPort`

`integer`

The external server port number.

`ExternalSSL`

`boolean`

If `true`, the system enables SSL for connections to the external server.

Default: `true`

`Host`

`string`

The Exchange server host name or IP address. Ignored if using OAuth.

`OAuth`

`boolean`

If `true`, the system enables OAuth for authentication. Don’t specify a password if `OAuth` is `true`. Available in macOS 10.14 and later

Default: `false`

`OAuthSignInURL`

`string`

The URL to load into a web view for authentication through OAuth when autodiscovery isn’t used. This setting requires a `Host` value.

`Password`

`string`

The password of the account. Use only with encrypted profiles.

`Path`

`string`

The server path.

`PayloadCertificateUUID`

`string`

The UUID of the certificate payload within the same profile to use for the identity credential. Supported on macOS 10.12 or later.

`Port`

`integer`

The server port number.

`SSL`

`boolean`

If `true`, the system enables SSL.

Default: `true`

`UserName`

`string`

The user name for this Exchange account. Required for noninteractive installation, such as through MDM. If missing, the system prompts the user for it during interactive profile installation.

## Discussion

Specify `com.apple.ews.account` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | \-    |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            EmailAddress
            juanchavez4@companyemail.com
            ExternalHost
            host.example.com
            ExternalPath

            ExternalSSL

            Host
            host.example.com
            MailNumberOfPastDaysToSync
            0
            Password
            Password123
            PayloadDisplayName
            Exchange Web Service
            PayloadIdentifier
            com.example.myewspayload
            PayloadType
            com.apple.ews.account
            PayloadUUID
            bb4adbbc-5516-45bb-bdee-cc7e47a5c5b5
            PayloadVersion
            1
            SSL

            UserName
            juanchavez4@companyemail.com

    PayloadDisplayName
    Exchange Web Service
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    ccb3eded-4486-4af8-81a3-add2d39cdfe7
    PayloadVersion
    1

```

## See Also

### Mail

object ExchangeActiveSync

The payload you use to configure Exchange ActiveSync accounts.

object Mail

The payload you use to configure a mail account on the device.

