

- Foundation
- AttributedString
-  init(localized:defaultValue:options:table:bundle:locale:comment:) 

Initializer

# init(localized:defaultValue:options:table:bundle:locale:comment:)

Creates an attributed string by looking up a localized string from the app’s bundle, using a default value if necessary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    localized key: StaticString,
    defaultValue: String.LocalizationValue,
    options: AttributedString.FormattingOptions = [],
    table: String? = nil,
    bundle: Bundle? = nil,
    locale: Locale? = nil,
    comment: StaticString? = nil
)
```

## Parameters 

`key`  

The key for a string in the table that `table` identifies.

`defaultValue`  

The localized string for the development locale. For other locales, the string uses this value if a localized string for `key` isn’t found in the table.

`options`  

Options that affect the handling of attributes.

`table`  

The bundle’s string table to search. If `table` is `nil` or is an empty string, the method attempts to use the table in `Localizable.strings`. The default is `nil`.

`bundle`  

The bundle to use for looking up strings. If `nil`, an app searches its main bundle. The default is `nil`.

`locale`  

The locale of the localized string to retrieve. If `nil`, this initializer uses the current locale. The default is `nil`.

`comment`  

The comment to place above the key-value pair in the strings file. This parameter provides the translator with some context about the localized string’s presentation to the user.

## Discussion

Use this initializer instead of init(localized:options:table:bundle:locale:comment:) if you prefer to use a symbolic string key, rather than use the development language’s string as the key.

## See Also

### Creating a Localized Attributed String with a Default Value

init&lt;S>(localized: StaticString, defaultValue: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?, including: S.Type)

Creates an attributed string by looking up a localized string from the app’s bundle, including an attribute scope, using a default value if necessary.

init&lt;S>(localized: StaticString, defaultValue: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?, including: KeyPath&lt;AttributeScopes, S.Type>)

Creates an attributed string by looking up a localized string from the app’s bundle, including an attribute scope that a key path identifies, using a default value if necessary.

