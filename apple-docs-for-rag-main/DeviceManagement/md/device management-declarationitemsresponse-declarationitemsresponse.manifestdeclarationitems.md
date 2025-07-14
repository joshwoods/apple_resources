

- Device Management
- DeclarationItemsResponse
-  DeclarationItemsResponse.ManifestDeclarationItems 

Object

# DeclarationItemsResponse.ManifestDeclarationItems

The dictionary that contains the lists of declarations available on the server.

Device Assignment ServicesVPP License Management

``` source
object DeclarationItemsResponse.ManifestDeclarationItems
```

## Properties

`Activations`

`[`ManifestDeclaration`]`

 (Required) 

The list of available activation declarations on the server.

`Assets`

`[`ManifestDeclaration`]`

 (Required) 

The list of available asset declarations on the server.

`Configurations`

`[`ManifestDeclaration`]`

 (Required) 

The list of available configuration declarations on the server.

`Management`

`[`ManifestDeclaration`]`

 (Required) 

The list of available management declarations on the server.

## See Also

### Supporting Objects

object ManifestDeclaration

A dictionary that describes a declaration.

