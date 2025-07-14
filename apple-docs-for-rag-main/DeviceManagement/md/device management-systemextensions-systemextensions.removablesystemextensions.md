

- Device Management
- SystemExtensions
-  SystemExtensions.RemovableSystemExtensions 

Device Management Profile

# SystemExtensions.RemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are removable.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object SystemExtensions.RemovableSystemExtensions
```

## Properties

`ANY`

`[string]`

The dictionary maps team identifiers (keys) to arrays of bundle identifiers, where the bundle identifier defines the system extension.

## Discussion

Available in macOS 12 and later.

## See Also

### Supporting Objects

object SystemExtensions.AllowedSystemExtensionTypes

A dictionary that maps team identifiers to system extensions.

object SystemExtensions.AllowedSystemExtensions

A dictionary that maps team identifiers to bundle identifiers that are allowed.

object SystemExtensions.NonRemovableFromUISystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.NonRemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

