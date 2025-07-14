

- Swift
- RegexComponent
-  localizedInteger(locale:) 

Type Method

# localizedInteger(locale:)

Creates a regex component that matches a localized numeric string, capturing it as an integer value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func localizedInteger(locale: Locale) -> Self
```

Available when `Self` is `IntegerFormatStyle`.

## Parameters 

`locale`  

The locale that specifies formatting conventions to use when matching numeric strings.

## Return Value

A `RegexComponent` that matches localized substrings as Int instances.

## Discussion

This method matches decimal substrings in accordance with the provided locale. For example, the value `1234567890` formats as `1,234,567,890` in the `en_US` locale, as `1 234 567 890` in the `FR` locale, and as `1234567890` in the `JP` locale. Because of this, the regex needs to know what locale convention to match against.

The following example creates a Regex that matches a date and time followed by whitespace and an integer formatted in the `en_US` locale. It then matches this regex against a source string containing a date with this format, some whitespace, and an integer value.

```
let enUSLocale = Locale(languageCode: .english, languageRegion: .unitedStates)
let source = "7/31/2022, 5:15:12 AM  49,525"
let matcher = Regex {
    One(.dateTime(date: .numeric,
                  time: .standard,
                  locale: enUSLocale,
                  timeZone: TimeZone(identifier: "PST")!))
    OneOrMore(.horizontalWhitespace)
    Capture {
        One(.localizedInteger(locale: enUSLocale))
    }
}
guard let match = source.firstMatch(of: matcher) else { return }
let matchedInteger = match?.1 // matchedInteger == 49525
```

## See Also

### Matching numeric formats

static func localizedDouble(locale: Locale) -> Self

Creates a regex component that matches a localized numeric string, capturing it as a double-precision floating-point value.

static func localizedDecimal(locale: Locale) -> Self

Creates a regex component that matches a localized decimal string, capturing it as a Foundation decimal.

static func localizedCurrency(code: Locale.Currency, locale: Locale) -> Self

Creates a regex component that matches a localized currency string, capturing it as a decimal value.

static func localizedIntegerCurrency(code: Locale.Currency, locale: Locale) -> Self

Creates a regex component that matches a localized currency string, capturing it as an integer value.

static func localizedIntegerPercentage(locale: Locale) -> Self

Creates a regex component that matches a localized percentage string, capturing it as a double-precision floating-point value.

static func localizedDoublePercentage(locale: Locale) -> Self

Creates a regex component that matches a localized percentage string, capturing it as a double-precision floating-point value.

