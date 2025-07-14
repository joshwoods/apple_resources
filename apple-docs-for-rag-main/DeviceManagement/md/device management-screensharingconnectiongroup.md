

- Device Management
-  ScreenSharingConnectionGroup 

Object

# ScreenSharingConnectionGroup

The declaration to configure a group of screen-sharing connections.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ScreenSharingConnectionGroup
```

## Properties

`ConnectionGroupUUID`

`string`

 (Required) 

A unique identifier for this connection group.

`GroupName`

`string`

 (Required) 

The name of the connection group.

`Members`

`[string]`

 (Required) 

An array of `ConnectionUUID`s that represent connections declared in `ScreenSharingConnection` configurations that are members of this group.

## Discussion

Specify `com.apple.configuration.screensharing.connection.group` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | macOS |
|------------------------------|-------|
| Allowed in User Enrollment   | macOS |
| Allowed in Local Enrollment  | macOS |
| Allowed in System Scope      | macOS |
| Allowed in User Scope        | macOS |

## See Also

### Supporting Objects

object ScreenSharingConnectionDisplayConfigurationObject

The display configuration for this connection.

object ScreenSharingHostSettings

The declaration to configure screen-sharing host settings and restrictions.

