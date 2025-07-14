

- Device Management
-  ExchangeActiveSync 

Device Management Profile

# ExchangeActiveSync

The payload you use to configure Exchange ActiveSync accounts.

iOS 4.0+iPadOS 4.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ExchangeActiveSync
```

## Properties

`allowMailDrop`

`boolean`

If `true`, the system enables this account to use Mail Drop.

Default: `false`

`Certificate`

`data`

The `.p12` identity certificate in NSData blob format, for accounts that allow authentication via certificate.

`CertificateName`

`string`

The name or description of the certificate.

`CertificatePassword`

`string`

The password necessary for the `.p12` identity certificate. Used with mandatory encryption of profiles.

`CommunicationServiceRules`

ExchangeActiveSync.CommunicationServiceRules

The communication service handler rules for this account.

`disableMailRecentsSyncing`

`boolean`

If `true`, the system excludes this account from Recent Addresses syncing.

Default: `false`

`EmailAddress`

`string`

The full email address for the account. If not present in the payload, the device prompts for this string during profile installation.

`HeaderMagic`

`string`

Deprecated 

The value of the `X-Apple-Config-Magic` header in each EAS HTTP request.

`Host`

`string`

The Exchange server host name or IP address.

If using OAuth without an OAuthSignInURL, the host name is ignored.

`MailNumberOfPastDaysToSync`

`integer`

The number of days in the past to sync mail on the device.

For no limit, use the value `0`.

Default: `7`

Possible Values: `0, 1, 3, 7, 14, 31`

`OAuth`

`boolean`

If `true`, enables OAuth for authentication. If enabled, don’t specify a password.

Available only in iOS 12.0 and above.

Default: `false`

`Password`

`string`

The password of the account. Use only with encrypted profiles.

`PayloadCertificateUUID`

`string`

The UUID of the certificate payload within the same profile to use for the identity credential. If this field is present, the Certificate field isn’t used.

`PreventAppSheet`

`boolean`

If `true`, prevents this account from sending mail in any app other than the Apple Mail app.

Default: `false`

`PreventMove`

`boolean`

If `true`, the system prevents moving messages from out of this email account into another account. This setting also prevents forwarding or replying from an account other than the recipient of the message.

Default: `false`

`SMIMEEnabled`

`boolean`

Deprecated 

If `true`, the system enables S/MIME encryption. In iOS 10.0 and later, this key is ignored. Use `SMIMESigningEnabled` instead.

Default: `false`

`SMIMEEncryptionEnabled`

`boolean`

Deprecated 

If `true`, the system enables S/MIME encryption for this account. Available in iOS 10.0 and later. As of iOS 12.0, this key is deprecated. Use `SMIMEEncryptByDefault` instead.

Default: `false`

`SMIMESigningEnabled`

`boolean`

If `true`, the system enables S/MIME signing for this account. Available in iOS 10.0 and later.

Default: `false`

`SMIMESigningUserOverrideable`

`boolean`

If `true`, the user can turn S/MIME signing on or off in Settings. Available in iOS 12.0 and later.

Default: `false`

`SMIMEEnableEncryptionPerMessageSwitch`

`boolean`

If `true`, the system displays the per-message encryption switch in the Mail Compose UI. Available in iOS 12.0 and later.

Default: `false`

`SMIMEEnablePerMessageSwitch`

`boolean`

Deprecated 

If `true`, the system displays the per-message encryption switch in the Mail Compose UI.

Available in iOS 8.0 and later. As of iOS 12.0, this key is deprecated. Use `SMIMEEnableEncryptionPerMessageSwitch` instead.

Default: `false`

`SMIMEEncryptByDefault`

`boolean`

If `true`, the system enables S/MIME encryption by default. If `SMIMEEnableEncryptionPerMessageSwitch` is `false`, the user can’t change this default. Available in iOS 12.0 and later.

Default: `false`

`SMIMEEncryptByDefaultUserOverrideable`

`boolean`

If `true`, the system enables encryption by default and the user can’t change it. Available in iOS 12.0 and later.

Default: `false`

`SMIMEEncryptionCertificateUUID`

`string`

The payload UUID of the identity certificate used to decrypt messages sent to this account. The system attaches the public certificate to outgoing mail to allow the user to receive encrypted mail. When the user sends encrypted mail, the system uses the public certificate to encrypt the copy of the mail in the user’s Sent mailbox.

`SMIMEEncryptionCertificateUUIDUserOverrideable`

`boolean`

If `true`, the user can select the S/MIME encryption identity, and encryption is on.Available in iOS 12.0 and later.

Default: `false`

`SMIMESigningCertificateUUID`

`string`

The UUID of the identity certificate used to sign messages sent from this account.

`SMIMESigningCertificateUUIDUserOverrideable`

`boolean`

If `true`, the user can select the signing identity. Available in iOS 12.0 and later.

Default: `false`

`SSL`

`boolean`

If `true`, the system enables SSL for authentication.

Default: `false`

`UserName`

`string`

This user name for this Exchange account. Required for noninteractive installations like MDM in iOS.

`EnableCalendars`

`boolean`

If `false`, the system disables the Calendars service for this account. The user can reenable Calendars service in Settings unless `EnableCalendarsUserOverridable` is `false`.

Note

At least of the following fields needs to be `true`: `EnableMail`, `EnableContacts`, `EnableCalendars`, `EnableReminders`, and `EnableNotes`.

Default: `true`

`EnableCalendarsUserOverridable`

`boolean`

If `false`, the system prevents the user from changing the state of the Calendars service for this account in Settings.

Default: `true`

`EnableContacts`

`boolean`

If `false`, the system disables the Contacts service for this account. The user can reenable Contacts service in Settings unless `EnableContactsUserOverridable` is `false`.

Note

At least of the following fields needs to be `true`: `EnableMail`, `EnableContacts`, `EnableCalendars`, `EnableReminders`, and `EnableNotes`.

Default: `true`

`EnableContactsUserOverridable`

`boolean`

If `false`, the system prevents the user from changing the state of the Contacts service for this account in Settings.

Default: `true`

`EnableMail`

`boolean`

If `false`, the system disables the Mail service for this account. The user can reenable Mail service in Settings unless `EnableMailUserOverridable` is `false`.

Note

At least of the following fields needs to be `true`: `EnableMail`, `EnableContacts`, `EnableCalendars`, `EnableReminders`, and `EnableNotes`.

Default: `true`

`EnableMailUserOverridable`

`boolean`

If `false`, the system prevents the user from changing the state of the Mail service for this account in Settings.

Default: `true`

`EnableNotes`

`boolean`

If `false`, the system disables the Notes service for this account. The user can reenable Notes service in Settings unless `EnableNotesUserOverridable` is `false`.

Note

At least of the following fields needs to be `true`: `EnableMail`, `EnableContacts`, `EnableCalendars`, `EnableReminders`, and `EnableNotes`.

Default: `true`

`EnableNotesUserOverridable`

`boolean`

If `false`, prevents the user from changing the state of the Notes service for this account in Settings.

Default: `true`

`EnableReminders`

`boolean`

If `false`, the system disables the Reminders service for this account. The user can reenable Reminders service in Settings unless `EnableRemindersUserOverridable` is `false`.

Note

At least of the following fields needs to be `true`: `EnableMail`, `EnableContacts`, `EnableCalendars`, `EnableReminders`, and `EnableNotes`.

Default: `true`

`EnableRemindersUserOverridable`

`boolean`

If `false`, the system prevents the user from changing the state of the Reminders service for this account in Settings.

Default: `true`

`OAuthSignInURL`

`string`

The URL that this account should use for signing in through OAuth. Ignored unless `OAuth` is `true`. If you specify this URL, auto-discovery isn’t used for this account, so you need to also specify a host.

`OAuthTokenRequestURL`

`string`

The URL that this account should use for token requests through OAuth. Ignored unless `OAuth` is `true`.

`OverridePreviousPassword`

`boolean`

If `true`, the system overrides the previous user/EAS password with the new EAS password in the payload. Available in iOS 14 and later.

Default: `false`

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.eas.account` as the payload type.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS              |
| User Channel               | Shared iPad      |
| Allow Manual Install       | iOS              |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | iOS              |
| Allow Multiple Payloads    | iOS, Shared iPad |

### Profile Example

```

    PayloadContent

            EmailAddress
            juanchavez4@companyemail.com
            EnableCalendars

            EnableCalendarsUserOverridable

            EnableContacts

            EnableContactsUserOverridable

            EnableMail

            EnableMailUserOverridable

            EnableNotes

            EnableNotesUserOverridable

            EnableReminders

            EnableRemindersUserOverridable

            Host
            host.companyemail.com
            MailNumberOfPastDaysToSync
            7
            OAuth

            OverridePreviousPassword

            SMIMEEnabled

            SMIMEEncryptionEnabled

            SMIMESigningEnabled

            SSL

            UserName
            juanchavez4@companyemail.com
            disableMailRecentsSyncing

            PayloadIdentifier
            com.example.myeaspayload
            PayloadType
            com.apple.eas.account
            PayloadUUID
            de789252-dcf2-42e7-91c8-0ab9f50aafc5
            PayloadVersion
            1

    PayloadDisplayName
    Exchange Active Sync
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b8fd6fd7-a55e-4eb1-96af-d9c4d8562e38'
    PayloadVersion
    1

```

## Topics

### Objects

object ExchangeActiveSync.CommunicationServiceRules

The communication service rules.

## See Also

### Mail

object ExchangeWebServices

The payload you use to configure an Exchange Web Services account for Contacts, Mail, Notes, Reminders, and Calendar.

object Mail

The payload you use to configure a mail account on the device.

