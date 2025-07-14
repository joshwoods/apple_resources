

- Device Management
-  ScreenSharingConnection 

Object

# ScreenSharingConnection

The declaration to configure a connection to a screen-sharing host.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ScreenSharingConnection
```

## Properties

`AuthenticationCredentialsAssetReference`

`string`

The identifier of an asset declaration that contains the required credentials for this connection to authenticate with the screen-sharing server. Set the corresponding asset type to `com.apple.asset.credential.userpassword`.

`ConnectionUUID`

`string`

 (Required) 

A unique identifier for this connection when it’s in a connection group.

`DisplayConfiguration`

ScreenSharingConnectionDisplayConfigurationObject

 (Required) 

The display configuration for this connection.

`DisplayName`

`string`

 (Required) 

The name of the connection.

`HostName`

`string`

 (Required) 

The host name or IP address of the Mac that hosts the screen-sharing connection.

`Port`

`integer`

The TCP port number on the host to initiate the connection.

## Discussion

Specify `com.apple.configuration.screensharing.connection` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | macOS |
|------------------------------|-------|
| Allowed in User Enrollment   | macOS |
| Allowed in Local Enrollment  | macOS |
| Allowed in System Scope      | macOS |
| Allowed in User Scope        | macOS |

## Topics

### Supporting Objects

object ScreenSharingConnectionDisplayConfigurationObject

The display configuration for this connection.

object ScreenSharingConnectionGroup

The declaration to configure a group of screen-sharing connections.

object ScreenSharingHostSettings

The declaration to configure screen-sharing host settings and restrictions.

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

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

