

- Foundation
- Bundle
-  localizedString(forKey:value:table:localizations:) 

Instance Method

# localizedString(forKey:value:table:localizations:)

Look up a localized string given a list of available languages.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func localizedString(
    forKey key: String,
    value: String?,
    table tableName: String?,
    localizations: [Locale.Language]
) -> String
```

## Parameters 

`key`  

The key for the localized string to retrieve.

`value`  

A default value to return if a localized string for `key` cannot be found.

`tableName`  

The name of the strings file to search. If `nil`, the method uses tables in `Localizable.strings`.

`localizations`  

An array of `Locale.Language` corresponding to available localizations. Bundle compares the array against its available localizations, and uses the best result to retrieve the localized string. If empty, we treat it as no localization is available, and may return a fallback.

## Return Value

A localized version of the string designated by `key` in table `tableName`.

