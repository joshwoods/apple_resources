

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Availability
-  unapprovedCount 

Instance Property

# unapprovedCount

The number of extensions not yet approved for hosting by the current app.

macOS 13.0+

``` source
let unapprovedCount: Int
```

## See Also

### Accessing Availability Information

var description: String

A string describing the extensions availability.

var totalCount: Int

The total number of installed extensions that the current app can host.

let disabledCount: Int

The number of extensions disabled for hosting in the current app.

let enabledCount: Int

The number of extensions enabled for hostng in the current app.

