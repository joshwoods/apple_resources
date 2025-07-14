

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Availability
-  enabledCount 

Instance Property

# enabledCount

The number of extensions enabled for hostng in the current app.

macOS 13.0+

``` source
let enabledCount: Int
```

## See Also

### Accessing Availability Information

var description: String

A string describing the extensions availability.

var totalCount: Int

The total number of installed extensions that the current app can host.

let disabledCount: Int

The number of extensions disabled for hosting in the current app.

let unapprovedCount: Int

The number of extensions not yet approved for hosting by the current app.

