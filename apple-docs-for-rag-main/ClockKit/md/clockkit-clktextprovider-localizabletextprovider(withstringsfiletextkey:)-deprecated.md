

- ClockKit
- CLKTextProvider
-  localizableTextProvider(withStringsFileTextKey:) Deprecated

Type Method

# localizableTextProvider(withStringsFileTextKey:)

Creates a localizable simple text provider using the strings file key for the text.

watchOS 3.0–9.0Deprecated

``` source
class func localizableTextProvider(withStringsFileTextKey textKey: String) -> Self
```

## Parameters 

`textKey`  

The key for the desired text. This key must appear in the localized string files named `ckcomplication.strings` in the WatchKit extension target.

## Return Value

A text provider object built from the specified arguments.

## Discussion

Use this method to create a text provider that returns localized strings.

## See Also

### Creating Localized Text Providers

class func localizableTextProvider(withStringsFileTextKey: String, shortTextKey: String?) -> Self

Creates a localizable simple text provider using strings file keys for both the regular text and the shorter fallback text.

Deprecated

class func localizableTextProvider(withStringsFileFormatKey: String, textProviders: [CLKTextProvider]) -> Self

Creates a localizable text provider with a strings file key that resolves to a format string, and with text providers for the replacement arguments.

Deprecated

