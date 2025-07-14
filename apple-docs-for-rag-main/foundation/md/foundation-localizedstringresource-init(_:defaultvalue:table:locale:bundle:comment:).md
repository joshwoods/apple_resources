

- Foundation
- LocalizedStringResource
-  init(\_:defaultValue:table:locale:bundle:comment:) 

Initializer

# init(\_:defaultValue:table:locale:bundle:comment:)

Creates a localized string resource from a static string and its bundle properties.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ key: StaticString,
    defaultValue: String.LocalizationValue,
    table: String? = nil,
    locale: Locale = .current,
    bundle: LocalizedStringResource.BundleDescription = .main,
    comment: StaticString? = nil
)
```

## Parameters 

`key`  

The key for an entry in the specified table.

`defaultValue`  

A localization value to use if `key` doesn’t exist in `table`. Xcode’s Product \> Export Localizations feature also extracts this value as the default translation in the project’s development locale.

`table`  

The name of the table containing the key-value pairs. If not provided, `nil`, or an empty string, this value defaults to `Localizable.strings.`

`locale`  

The locale for the resource to use. By default, the resource uses current.

`bundle`  

A LocalizedStringResource.BundleDescription that indicates where to locate the table’s strings file. By default, the resource uses the main bundle.

`comment`  

The comment to place above the key-value pair in the strings file. This parameter provides the translator with some context about the localized string’s presentation to the user.

## See Also

### Creating a localized string resource

init(String.LocalizationValue, table: String?, locale: Locale, bundle: LocalizedStringResource.BundleDescription, comment: StaticString?)

Creates a localized string resource from a localization key and its bundle properties.

