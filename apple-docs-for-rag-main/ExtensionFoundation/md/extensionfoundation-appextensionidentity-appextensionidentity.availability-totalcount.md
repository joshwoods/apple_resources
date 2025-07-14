

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Availability
-  totalCount 

Instance Property

# totalCount

The total number of installed extensions that the current app can host.

macOS 13.0+

``` source
var totalCount: Int { get }
```

## See Also

### Accessing Availability Information

var description: String

A string describing the extensions availability.

let disabledCount: Int

The number of extensions disabled for hosting in the current app.

let enabledCount: Int

The number of extensions enabled for hostng in the current app.

let unapprovedCount: Int

The number of extensions not yet approved for hosting by the current app.

