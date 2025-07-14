

- FSKit
-  FSModuleIdentity 

Class

# FSModuleIdentity

An installed file system module.

macOS 15.4+

``` source
class FSModuleIdentity
```

## Topics

### Accessing module properties

var bundleIdentifier: String

The module’s bundle identifier.

var url: URL

The module’s URL.

var isEnabled: Bool

A Boolean value that indicates if the module is enabled.

### Default Implementations

Identifiable Implementations

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSObjectProtocol

## See Also

### Discovering installed extensions

func fetchInstalledExtensions(completionHandler: ([FSModuleIdentity]?, (any Error)?) -> Void)

Asynchronously retrieves an list of installed file system modules.

