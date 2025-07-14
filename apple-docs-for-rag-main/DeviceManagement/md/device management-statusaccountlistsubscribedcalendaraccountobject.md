

- Device Management
-  StatusAccountListSubscribedCalendarAccountObject 

Object

# StatusAccountListSubscribedCalendarAccountObject

A status report of the client’s calendar account details.

iOS 16.0+iPadOS 16.0+macOS 14.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object StatusAccountListSubscribedCalendarAccountObject
```

## Properties

`_removed`

`boolean`

If `true`, the app is removed and the status item object only contains this key and the `identifier` key.

Default: `false`

`calendar-url`

`string`

The URL of the subscribed calendar.

`declaration-identifier`

`string`

The identifier of the declaration that installed the account. Only present if a declaration installed the account.

`identifier`

`string`

 (Required) 

The unique identifier for the account.

`is-enabled`

`boolean`

A Boolean value that indicates whether the Calendar app displays this calendar.

`username`

`string`

The user name for the account.

`visible-name`

`string`

The name of the account.

