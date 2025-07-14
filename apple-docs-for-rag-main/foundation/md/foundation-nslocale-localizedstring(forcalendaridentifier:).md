

- Foundation
- NSLocale
-  localizedString(forCalendarIdentifier:) 

Instance Method

# localizedString(forCalendarIdentifier:)

Returns the localized string for the specified calendar identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func localizedString(forCalendarIdentifier calendarIdentifier: String) -> String?
```

## Parameters 

`calendarIdentifier`  

The calendar identifier indicating the calendar whose name you want. Use one of the values listed in `Calendar Identifiers`.

## Return Value

A human readable string suitable for display to the user corresponding to the given calendar.

## Discussion

For example, on an American English (`en_US`) locale, passing gregorian as the identifier, produces the string `"Gregorian Calendar"`.

## See Also

### Getting Display Information About a Locale

func localizedString(forLocaleIdentifier: String) -> String

Returns the localized string for the specified locale identifier.

func localizedString(forCountryCode: String) -> String?

Returns the localized string for a country or region code.

func localizedString(forLanguageCode: String) -> String?

Returns the localized string for the specified language code.

func localizedString(forScriptCode: String) -> String?

Returns the localized string for the specified script code.

func localizedString(forVariantCode: String) -> String?

Returns the localized string for the specified variant code.

func localizedString(forCollationIdentifier: String) -> String?

Returns the localized string for the specified collation identifier.

func localizedString(forCollatorIdentifier: String) -> String?

Returns the localized string for the specified collator identifier.

func localizedString(forCurrencyCode: String) -> String?

Returns the localized string for the specified currency code.

Locale Calendar Identifiers

The types of calendars.

