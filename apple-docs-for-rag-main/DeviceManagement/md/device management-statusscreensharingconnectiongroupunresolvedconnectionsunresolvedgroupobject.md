

- Device Management
-  StatusScreenSharingConnectionGroupUnresolvedConnectionsUnresolvedGroupObject 

Object

# StatusScreenSharingConnectionGroupUnresolvedConnectionsUnresolvedGroupObject

A status item that contains an unresolved connection group.

macOS 14.1+Device Assignment ServicesVPP License Management

``` source
object StatusScreenSharingConnectionGroupUnresolvedConnectionsUnresolvedGroupObject
```

## Properties

`_removed`

`boolean`

If `true`, the system removed the unresolved connection group and only this key and the `identifier` key are present in the status item object.

Default: `false`

`identifier`

`string`

 (Required) 

The unique `ConnectionGroupUUID` identifier of the connection group.

`unresolved_connections`

`[string]`

An array of `ConnectionUUID` values specifed in the `Members` key in the group’s declaration for the unresolved connections.

