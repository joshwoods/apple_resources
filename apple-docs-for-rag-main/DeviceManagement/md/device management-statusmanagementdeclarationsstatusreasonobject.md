

- Device Management
-  StatusManagementDeclarationsStatusReasonObject 

Object

# StatusManagementDeclarationsStatusReasonObject

The details of an error in a status report.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementDeclarationsStatusReasonObject
```

## Properties

`code`

`string`

 (Required) 

The error code for this error.

`description`

`string`

The description for this error.

`details`

StatusManagementDeclarationsStatusReason_DetailsObject

A dictionary that contains further details about this error.

## See Also

### Supporting Objects

object StatusManagementDeclarationsDeclarationsObject

A collection of the client’s processed declarations.

object StatusManagementDeclarationsDeclarationObject

A processed declaration for the client.

object StatusManagementDeclarationsStatusReason_DetailsObject

A dictionary that contains further details about an error.

