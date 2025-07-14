

- ExtensionFoundation
- AppExtensionIdentity
-  localizedName 

Instance Property

# localizedName

A localized, human-readable name for the extension.

macOS 13.0+

``` source
var localizedName: String { get }
```

## See Also

### Identifying the Process

var bundleIdentifier: String

The bundle identifier for the extension.

var extensionPointIdentifier: String

A unique identifier for the extension point this extension targets.

struct Identities

An asynchronous sequence that returns the enabled extensions that match provided constraints.

