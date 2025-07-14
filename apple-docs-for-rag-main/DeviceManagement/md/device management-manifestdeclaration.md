

- Device Management
-  ManifestDeclaration 

Object

# ManifestDeclaration

A dictionary that describes a declaration.

Device Assignment ServicesVPP License Management

``` source
object ManifestDeclaration
```

## Properties

`Identifier`

`string`

 (Required) 

The declaration’s identifier.

`ServerToken`

`string`

 (Required) 

The `ServerToken` value of the declaration.

The client uses this to determine if the actual payload is different from the one on the client. Servers must compute the token over the entire declaration content to ensure the value always changes whenever there’s any change to the content.

## See Also

### Supporting Objects

object DeclarationItemsResponse.ManifestDeclarationItems

The dictionary that contains the lists of declarations available on the server.

