

- Device Management
- SystemExtensions
-  SystemExtensions.AllowedSystemExtensionTypes 

Device Management Profile

# SystemExtensions.AllowedSystemExtensionTypes

A dictionary that maps team identifiers to system extensions.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object SystemExtensions.AllowedSystemExtensionTypes
```

## Properties

`ANY`

`[string]`

The mapping of team identifier to an array of strings, where each string is a type of system extension that may be installed for that team identifier.

## See Also

### Supporting Objects

object SystemExtensions.AllowedSystemExtensions

A dictionary that maps team identifiers to bundle identifiers that are allowed.

object SystemExtensions.NonRemovableFromUISystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.NonRemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.RemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are removable.

