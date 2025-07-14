

- Device Management
-  StatusServicesBackgroundTaskBackgroundTaskObject 

Object

# StatusServicesBackgroundTaskBackgroundTaskObject

A status report of a background task.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object StatusServicesBackgroundTaskBackgroundTaskObject
```

## Properties

`_removed`

`boolean`

If `true`, the app is removed and the status item object only contains this key and the `identifier` key.

Default: `false`

`code-signature`

`string`

For types other than `agent` or `daemon`, this is the code signature designated requirement of the item, if available.

`identifier`

`string`

 (Required) 

The background task UUID which the system uses as the primary key.

`launchd`

StatusServicesBackgroundTaskBackgroundTask_LaunchdObject

Details about a `launchd`-based background task, which is only present when the type is `daemon` or `agent`.

`path`

`string`

 (Required) 

For an `agent` or `daemon`, the path to the `launchd` `plist` file. For other types, the path to the app or the document.

`state`

`string`

 (Required) 

The SMAppService.Status enumeration.

Possible Values: `not-registered, enabled, requires-approval, not-found`

`type`

`string`

 (Required) 

The daemon, agent, or SFL login item type.

Possible Values: `daemon, agent, login-item, app, user-item`

`uid`

`integer`

 (Required) 

The numeric user identifier of the owner of the background task.

## See Also

### Supporting Objects

object StatusServicesBackgroundTaskBackgroundTask_LaunchdObject

A status report of a background task that’s based on a launch daemon.

object StatusServicesBackgroundTaskBackgroundTask_Launchd_DeviceManagementObject

