

- Device Management
-  StatusServicesBackgroundTaskBackgroundTask_LaunchdObject 

Object

# StatusServicesBackgroundTaskBackgroundTask_LaunchdObject

A status report of a background task that’s based on a launch daemon.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object StatusServicesBackgroundTaskBackgroundTask_LaunchdObject
```

## Properties

`checksum`

`string`

 (Required) 

The hash value of the `launchd` `plist` file.

`device-management`

StatusServicesBackgroundTaskBackgroundTask_Launchd_DeviceManagementObject

`label`

`string`

 (Required) 

The label of the `launchd`-based background task.

`program`

`string`

 (Required) 

The program that the `launchd` `plist` file specifies.

`program-arguments`

`[string]`

The program arguments that the `launchd` `plist` file specifies.

## See Also

### Supporting Objects

object StatusServicesBackgroundTaskBackgroundTaskObject

A status report of a background task.

object StatusServicesBackgroundTaskBackgroundTask_Launchd_DeviceManagementObject

