

- PackageDescription
- Package
- Package.Dependency
-  name Deprecated

Instance Property

# name

The name of the dependency.

SwiftPMDeprecated

``` source
var name: String? { get }
```

Deprecated

use kind instead

## Discussion

If the `name` is `nil`, Swift Package Manager deduces the dependency’s name from its package identity or Git URL.

