

- ExtensionFoundation
- AppExtensionIdentity
-  AppExtensionIdentity.Availability 

Structure

# AppExtensionIdentity.Availability

An object that contains information about available extensions.

macOS 13.0+

``` source
struct Availability
```

## Topics

### Creating an Availability Object

init()

Creates an app extension identity availability object.

### Accessing Availability Information

var description: String

A string describing the extensions availability.

var totalCount: Int

The total number of installed extensions that the current app can host.

let disabledCount: Int

The number of extensions disabled for hosting in the current app.

let enabledCount: Int

The number of extensions enabled for hostng in the current app.

let unapprovedCount: Int

The number of extensions not yet approved for hosting by the current app.

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Monitoring Extensions

static var availabilityUpdates: AsyncStream&lt;AppExtensionIdentity.Availability>

