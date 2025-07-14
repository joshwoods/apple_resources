

- Device Management
-  ManagementStatusSubscriptions 

Object

# ManagementStatusSubscriptions

The declaration to configure status subscriptions.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagementStatusSubscriptions
```

## Properties

`StatusItems`

`[`ManagementStatusSubscriptionsStatusItemObject`]`

 (Required) 

An array of status items that the device notifies subscribers about.

## Mentioned in 

Leveraging the declarative management data model to scale devices

## Discussion

Specify `com.apple.configuration.management.status-subscriptions` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS, tvOS, watchOS              |
|------------------------------|----------------------------------------|
| Allowed in User Enrollment   | iOS, macOS                             |
| Allowed in Local Enrollment  | iOS, macOS, tvOS, watchOS              |
| Allowed in System Scope      | iOS, macOS, Shared iPad, tvOS, watchOS |
| Allowed in User Scope        | macOS, Shared iPad                     |

## Topics

### Supporting Objects

object ManagementStatusSubscriptionsStatusItemObject

The declaration for configuring a specific status subscription.

## See Also

### Configurations

object AccountCalDAV

The declaration to configure a Calendar account.

object AccountCardDAV

The declaration to configure an address book account.

object AccountExchange

The declaration to configure an Exchange account.

object AccountGoogle

The declaration to configure a Google account.

object AccountLDAP

The declaration to configure a Lightweight Directory Access Protocol (LDAP) account.

object AccountMail

The declaration to configure a Mail account.

object AccountSubscribedCalendar

The declaration to configure a Calendar subscription.

object AppManaged

The declaration to configure a managed app.

object DiskManagementSettings

The declaration to configure disk management settings on the device.

object LegacyInteractiveProfile

The declaration to configure an interactive, legacy profile.

object LegacyProfile

The declaration to configure a legacy profile.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

object SafariExtensionSettings

The declaration to configure Safari Extensions.

