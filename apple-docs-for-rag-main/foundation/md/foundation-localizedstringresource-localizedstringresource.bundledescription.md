

- Foundation
- LocalizedStringResource
-  LocalizedStringResource.BundleDescription 

Enumeration

# LocalizedStringResource.BundleDescription

The location of a bundle to use for looking up localized strings, such as the main bundle, or a bundle at a specific file URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum BundleDescription
```

## Topics

### Bundle descriptions

case main

The app’s main bundle.

case atURL(URL)

A bundle located at a specific file URL.

case forClass(AnyClass)

The bundle for a specific class.

## Relationships

### Conforms To

- Sendable

## See Also

### Accessing resource properties

let key: String

The key to use to look up a localized string.

let defaultValue: String.LocalizationValue

The resource’s default value.

let table: String?

The name of the table containing the key-value pairs.

var bundle: LocalizedStringResource.BundleDescription

The bundle containing the table’s strings file.

var locale: Locale

The locale to use to look up the localized string from the string resource.

