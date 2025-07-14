

- Device Management
-  APN 

Device Management Profile

# APN

The payload you use to configure access point names.

iOS 4.0–7.0DeprecatediPadOS 4.0–7.0DeprecatedDevice Assignment ServicesVPP License Management

``` source
object APN
```

## Properties

`DefaultsData`

APN.DefaultsData

Deprecated   (Required) 

The list of access point names (APNs).

`DefaultsDomainName`

`string`

Deprecated   (Required) 

The domain name.

Value: `com.apple.managedCarrier`

## Discussion

This profile is deprecated. Use the Cellular profile instead.

Specify `com.apple.apn.managed` as the payload type.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Allow Manual Install       | iOS, watchOS     |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | \-               |
| Allow Multiple Payloads    | \-               |

## Topics

### Objects

object APN.DefaultsData

An array of access point name dictionaries.

## See Also

### Deprecated

object AIMAccount

The payload you use to configure an AIM account on the device.

object FDERecoveryKeyRedirection

The payload you use to configure FileVault recovery key redirection.

object JabberAccount

The payload you use to configure a Jabber account.

object MacOSServerAccount

The payload you use to configure a macOS server account.

object MediaManagementAllowedMedia

The payload you use to configure media management.

object ParentalControlsDashboardWidgetRestrictions

The payload you use to configure the parental control dashboard allow list.

object ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

object ShareKit

The payload you use to configure ShareKit.

object SystemPreferences

The payload you use to configure the preference panes.

