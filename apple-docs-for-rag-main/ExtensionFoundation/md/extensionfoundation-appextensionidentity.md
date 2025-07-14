

- ExtensionFoundation
-  AppExtensionIdentity 

Structure

# AppExtensionIdentity

An object that uniquely identifies an app extension.

macOS 13.0+

``` source
struct AppExtensionIdentity
```

## Topics

### Identifying the Process

var bundleIdentifier: String

The bundle identifier for the extension.

var extensionPointIdentifier: String

A unique identifier for the extension point this extension targets.

var localizedName: String

A localized, human-readable name for the extension.

struct Identities

An asynchronous sequence that returns the enabled extensions that match provided constraints.

### Monitoring Extensions

struct Availability

An object that contains information about available extensions.

static var availabilityUpdates: AsyncStream&lt;AppExtensionIdentity.Availability>

### Comparing Extensions

func hash(into: inout Hasher)

Hashes the essential components of the extension by feeding them into the given hash function.

static func == (AppExtensionIdentity, AppExtensionIdentity) -> Bool

Indicates whether two extensions are equal

### Type Methods

static func matching(appExtensionPointIDs: String...) throws -> AppExtensionIdentity.Identities

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### App Extensions

protocol AppExtension

Declares a type used by app extensions.

protocol AppExtensionConfiguration

An object that holds configuration options for an app extension.

