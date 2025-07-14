

- Device Management
-  ScreenSharingConnectionDisplayConfigurationObject 

Object

# ScreenSharingConnectionDisplayConfigurationObject

The display configuration for this connection.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ScreenSharingConnectionDisplayConfigurationObject
```

## Properties

`DisplayType`

`string`

 (Required) 

The type of display for the connection, which has these allowed values:

`Virtual1`  
Create one virtual display.

`Virtual2`  
Create two virtual displays.

Possible Values: `Virtual1, Virtual2`

## See Also

### Supporting Objects

object ScreenSharingConnectionGroup

The declaration to configure a group of screen-sharing connections.

object ScreenSharingHostSettings

The declaration to configure screen-sharing host settings and restrictions.

