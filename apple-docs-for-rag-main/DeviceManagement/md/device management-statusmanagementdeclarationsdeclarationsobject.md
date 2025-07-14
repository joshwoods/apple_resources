

- Device Management
-  StatusManagementDeclarationsDeclarationsObject 

Object

# StatusManagementDeclarationsDeclarationsObject

A collection of the client’s processed declarations.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementDeclarationsDeclarationsObject
```

## Properties

`activations`

`[`StatusManagementDeclarationsDeclarationObject`]`

 (Required) 

An array of declarations that represent the client’s processed activation types.

`assets`

`[`StatusManagementDeclarationsDeclarationObject`]`

 (Required) 

An array of declarations that represent the client’s processed assets.

`configurations`

`[`StatusManagementDeclarationsDeclarationObject`]`

 (Required) 

An array of declarations that represent the client’s processed configuration types.

`management`

`[`StatusManagementDeclarationsDeclarationObject`]`

 (Required) 

An array of declarations that represent the client’s processed declaration types.

## See Also

### Supporting Objects

object StatusManagementDeclarationsDeclarationObject

A processed declaration for the client.

object StatusManagementDeclarationsStatusReasonObject

The details of an error in a status report.

object StatusManagementDeclarationsStatusReason_DetailsObject

A dictionary that contains further details about an error.

