

- Device Management
- SystemExtensions
-  SystemExtensions.AllowedSystemExtensions 

Device Management Profile

# SystemExtensions.AllowedSystemExtensions

A dictionary that maps team identifiers to bundle identifiers that are allowed.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object SystemExtensions.AllowedSystemExtensions
```

## Properties

`ANY`

`[string]`

The mapping of team identifiers to arrays of bundle identifiers, where the bundle identifier is that of the system extension to be installed.

## See Also

### Supporting Objects

object SystemExtensions.AllowedSystemExtensionTypes

A dictionary that maps team identifiers to system extensions.

object SystemExtensions.NonRemovableFromUISystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.NonRemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.RemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are removable.

