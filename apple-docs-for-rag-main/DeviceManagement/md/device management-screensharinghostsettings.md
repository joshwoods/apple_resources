

- Device Management
-  ScreenSharingHostSettings 

Object

# ScreenSharingHostSettings

The declaration to configure screen-sharing host settings and restrictions.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ScreenSharingHostSettings
```

## Properties

`MaximumVirtualDisplays`

`integer`

The maximum number of virtual displays to make available to clients.

Minimum: `0`

Maximum: `2`

`PortBase`

`integer`

The initial UDP port number to connect to the host. Screen sharing requires multiple connections, so the system increments this value by 1 for each additional connection. This doesn’t change the port number that the system uses to initially establish a connection with a host, which is always TCP port 5900.

Minimum: `1024`

Maximum: `65535`

`PreventCopyFilesFromHost`

`boolean`

If `true`, the system prevents users from copying files from the screen-sharing host.

Default: `false`

`PreventCopyFilesToHost`

`boolean`

If `true`, the system prevents users from copying files to the screen-sharing host.

Default: `false`

`PreventHighPerformanceConnections`

`boolean`

If `true`, the system prevents clients from establishing high-performance connections to the host.

Default: `false`

## Discussion

Specify `com.apple.configuration.screensharing.host.settings` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | macOS |
|------------------------------|-------|
| Allowed in User Enrollment   | \-    |
| Allowed in Local Enrollment  | macOS |
| Allowed in System Scope      | macOS |
| Allowed in User Scope        | \-    |

## See Also

### Supporting Objects

object ScreenSharingConnectionDisplayConfigurationObject

The display configuration for this connection.

object ScreenSharingConnectionGroup

The declaration to configure a group of screen-sharing connections.

