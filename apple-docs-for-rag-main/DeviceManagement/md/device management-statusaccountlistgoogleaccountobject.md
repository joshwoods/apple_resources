

- Device Management
-  StatusAccountListGoogleAccountObject 

Object

# StatusAccountListGoogleAccountObject

A status report of the client’s Google account details.

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object StatusAccountListGoogleAccountObject
```

## Properties

`_removed`

`boolean`

If `true`, the app is removed and the status item object only contains this key and the `identifier` key.

Default: `false`

`are-calendars-enabled`

`boolean`

A Boolean value that indicates whether the Calendar app displays calendars and events for this account.

`are-contacts-enabled`

`boolean`

A Boolean value that indicates whether the Contacts app displays contacts for this account.

`are-notes-enabled`

`boolean`

A Boolean value that indicates whether the Notes app displays notes for this account.

`declaration-identifier`

`string`

The identifier of the declaration that installed the account. Only present if a declaration installed the account.

`identifier`

`string`

 (Required) 

The unique identifier for the account.

`is-mail-enabled`

`boolean`

A Boolean value that indicates whether the Mail app displays mail for this account.

`username`

`string`

The user name for the account.

`visible-name`

`string`

The name of the account.

