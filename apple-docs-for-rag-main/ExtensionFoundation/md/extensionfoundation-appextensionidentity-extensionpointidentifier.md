

- ExtensionFoundation
- AppExtensionIdentity
-  extensionPointIdentifier 

Instance Property

# extensionPointIdentifier

A unique identifier for the extension point this extension targets.

macOS 13.0+

``` source
var extensionPointIdentifier: String { get }
```

## See Also

### Identifying the Process

var bundleIdentifier: String

The bundle identifier for the extension.

var localizedName: String

A localized, human-readable name for the extension.

struct Identities

An asynchronous sequence that returns the enabled extensions that match provided constraints.

