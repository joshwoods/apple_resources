

- Device Management
-  StatusAccountListCalDAVAccountObject 

Object

# StatusAccountListCalDAVAccountObject

A status report of the client’s CalDAV account details.

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object StatusAccountListCalDAVAccountObject
```

## Properties

`_removed`

`boolean`

If `true`, the app is removed and the status item object only contains this key and the `identifier` key.

Default: `false`

`are-calendars-enabled`

`boolean`

If `true`, the Calendar app is displaying calendars and events for the account.

`are-reminders-enabled`

`boolean`

If `true`, the Reminders app is displaying reminders for the account.

`declaration-identifier`

`string`

The identifier of the declaration that installed the account. Only present if a declaration installed the account.

`hostname`

`string`

The server host name for the account.

`identifier`

`string`

 (Required) 

The unique identifier for the account.

`port`

`integer`

The server port for the account.

`username`

`string`

The user name for the account.

`visible-name`

`string`

The name of the account.

