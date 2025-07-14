

- Device Management
-  StatusManagementDeclarationsDeclarationObject 

Object

# StatusManagementDeclarationsDeclarationObject

A processed declaration for the client.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementDeclarationsDeclarationObject
```

## Properties

`active`

`boolean`

 (Required) 

If `true`, the declaration is active on the device.

`identifier`

`string`

 (Required) 

The `identifier` of the declaration this status report refers to.

`reasons`

`[`StatusManagementDeclarationsStatusReasonObject`]`

The details of any client errors.

`server-token`

`string`

 (Required) 

The `ServerToken` of the declaration this status report refers to.

`valid`

`string`

 (Required) 

This string defines the validity of the declaration. If it’s `invalid`, the `reasons` property contains more details.

Possible Values: `unknown, invalid, valid`

## See Also

### Supporting Objects

object StatusManagementDeclarationsDeclarationsObject

A collection of the client’s processed declarations.

object StatusManagementDeclarationsStatusReasonObject

The details of an error in a status report.

object StatusManagementDeclarationsStatusReason_DetailsObject

A dictionary that contains further details about an error.

