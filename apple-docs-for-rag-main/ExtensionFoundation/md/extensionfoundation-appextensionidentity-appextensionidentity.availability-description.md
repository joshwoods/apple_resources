

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Availability
-  description 

Instance Property

# description

A string describing the extensions availability.

macOS 13.0+

``` source
var description: String { get }
```

## See Also

### Accessing Availability Information

var totalCount: Int

The total number of installed extensions that the current app can host.

let disabledCount: Int

The number of extensions disabled for hosting in the current app.

let enabledCount: Int

The number of extensions enabled for hostng in the current app.

let unapprovedCount: Int

The number of extensions not yet approved for hosting by the current app.

