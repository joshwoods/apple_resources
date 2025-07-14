

- Device Management
-  DeclarationItemsResponse 

Object

# DeclarationItemsResponse

The set of available declarations on the server.

Device Assignment ServicesVPP License Management

``` source
object DeclarationItemsResponse
```

## Properties

`Declarations`

DeclarationItemsResponse.ManifestDeclarationItems

 (Required) 

The set of available declarations on the server.

`DeclarationsToken`

`string`

 (Required) 

The current value of the declarations token. Clients use this to detect when declarations change so they can refetch the token.

## Topics

### Supporting Objects

object DeclarationItemsResponse.ManifestDeclarationItems

The dictionary that contains the lists of declarations available on the server.

object ManifestDeclaration

A dictionary that describes a declaration.

