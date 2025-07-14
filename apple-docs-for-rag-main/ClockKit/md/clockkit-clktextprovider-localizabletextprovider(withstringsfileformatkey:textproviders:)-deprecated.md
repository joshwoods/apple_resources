

- ClockKit
- CLKTextProvider
-  localizableTextProvider(withStringsFileFormatKey:textProviders:) Deprecated

Type Method

# localizableTextProvider(withStringsFileFormatKey:textProviders:)

Creates a localizable text provider with a strings file key that resolves to a format string, and with text providers for the replacement arguments.

watchOS 3.0–9.0Deprecated

``` source
class func localizableTextProvider(
    withStringsFileFormatKey formatKey: String,
    textProviders: [CLKTextProvider]
) -> Self
```

## Parameters 

`formatKey`  

The key for the localized format string. This key must appear in the localized string files named `ckcomplication.strings` in the WatchKit extension target.

Since the format string’s replacement arguments come from other text providers, the only allowable format specifiers are `%@` and variants (for example, reordering specifiers like `%1@` are also supported).

`textProviders`  

The text providers that produce the format string’s replacement arguments.

## Return Value

A text provider object built from the specified arguments.

## Discussion

Use this method to create a compound text provider using a format string, with other text providers to provide the replacement arguments.

## See Also

### Creating Localized Text Providers

class func localizableTextProvider(withStringsFileTextKey: String) -> Self

Creates a localizable simple text provider using the strings file key for the text.

Deprecated

class func localizableTextProvider(withStringsFileTextKey: String, shortTextKey: String?) -> Self

Creates a localizable simple text provider using strings file keys for both the regular text and the shorter fallback text.

Deprecated

