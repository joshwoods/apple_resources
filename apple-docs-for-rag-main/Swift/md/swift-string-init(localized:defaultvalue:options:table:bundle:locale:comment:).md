

- Swift
- String
-  init(localized:defaultValue:options:table:bundle:locale:comment:) 

Initializer

# init(localized:defaultValue:options:table:bundle:locale:comment:)

Creates a localized string from an arbitrary static string key, applying the specified options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    localized key: StaticString,
    defaultValue: String.LocalizationValue,
    options: String.LocalizationOptions,
    table: String? = nil,
    bundle: Bundle? = nil,
    locale: Locale = .current,
    comment: StaticString? = nil
)
```

## Parameters 

`defaultValue`  

A default value to use if looking up a localized string from the bundle fails. This is typically the localizable string in the development language.

`options`  

A localization options instance that specifies localization options to apply, such as replacement values for formatted strings.

`table`  

The bundle’s string table to search. If `table` is `nil` or is an empty string, the method attempts to use the table named `Localizable`. The default is `nil`.

`bundle`  

The bundle to use for looking up strings. If `nil`, an app searches its main bundle. The default is `nil`.

`locale`  

The locale to use when localizing interpolated values, such as numbers. This doesn’t change which locale the system uses to look up the localized string. If `nil`, this initializer uses the current locale. The default is `nil`.

`comment`  

The comment to place above the key-value pair in the strings file. This parameter provides the translator with some context about the localized string’s presentation to the user.

## Discussion

Use the `defaultValue` initializers when you want to use an explicit *key* to look up localized strings. This is useful if the localizable string in your development language is ambiguous. For example *call* in English can be a noun or a verb. In this case, you might want to use `.strings` file entries like `CALL_NOUN` and `CALL_VERB` to disambiguate the uses for localizers. You then use this initializer, providing both a key and a default value to use if the system can’t find the key at runtime.

```
// Assume the strings file or catalog contains the following:
// English: CALL_VERB = "Call", CALL_NOUN = "Call"
// French: CALL_VERB = "Appeler", CALL_NOUN = "Appel"
let callVerb = String(localized: "CALL_VERB", defaultValue: "Call")
let callNoun = String(localized: "CALL_NOUN", defaultValue: "Call")
// callVerb == "Call" in en locale, "Appeler" in fr locale.
// callNoun == "Call" in en locale, "Appel" in fr locale.
```

Use the `options` parameter to include any replacement values to insert into the localized formatted string. The following example shows how to insert strongly-typed replacement values into a string:

```
// Assume the strings file or catalog contains the explicit key "POSITION_IN_QUEUE",
// with localizations "Position in queue: %lld." for English and
// "Position dans la file d’attente: %lld." for French.
var options = String.LocalizationOptions()
options.replacements = [12]
let localized = String (localized: "POSITION_IN_QUEUE",
                        defaultValue:"Position in queue: \(placeholder: .int).",
                        options: options)
// localized = "Position in queue: 12." in en locale, "Position dans la file d’attente: 12." in fr locale.
```

To use the default localization as the key rather than an explicit key, use init(localized:options:table:bundle:locale:comment:) instead. If you need to provide localized strings to another process that might be using a different locale, use init(localized:options:).

## See Also

### Creating a Localized String

init(localized: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string.

init(localized: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string, applying the specified options.

struct LocalizationValue

A reference to a localizable string, with optional string interpolation.

struct LocalizationOptions

Options to apply when initializing a localized string.

init(localized: StaticString, defaultValue: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key.

init(localized: LocalizedStringResource)

Creates a localized string from a localized string resource.

init(localized: LocalizedStringResource, options: String.LocalizationOptions)

Creates a localized string from a localized string resource, applying the specified options.

