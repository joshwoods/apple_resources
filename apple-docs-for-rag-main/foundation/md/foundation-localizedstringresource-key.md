

- Foundation
- LocalizedStringResource
-  key 

Instance Property

# key

The key to use to look up a localized string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let key: String
```

## See Also

### Accessing resource properties

let defaultValue: String.LocalizationValue

The resource’s default value.

let table: String?

The name of the table containing the key-value pairs.

var bundle: LocalizedStringResource.BundleDescription

The bundle containing the table’s strings file.

enum BundleDescription

The location of a bundle to use for looking up localized strings, such as the main bundle, or a bundle at a specific file URL.

var locale: Locale

The locale to use to look up the localized string from the string resource.

