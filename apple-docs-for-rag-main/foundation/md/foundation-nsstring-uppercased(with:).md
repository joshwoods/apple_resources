

- Foundation
- NSString
-  uppercased(with:) 

Instance Method

# uppercased(with:)

Returns a version of the string with all letters converted to uppercase, taking into account the specified locale.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func uppercased(with locale: Locale?) -> String
```

## Parameters 

`locale`  

The locale. For strings presented to users, pass the current locale (\[NSLocale current\]). To use the system locale, pass `nil`.

## Return Value

An uppercase string using the `locale`.

## See Also

### Changing Case

var lowercased: String

A lowercase representation of the string.

var localizedLowercase: String

Returns a version of the string with all letters converted to lowercase, taking into account the current locale.

func lowercased(with: Locale?) -> String

Returns a version of the string with all letters converted to lowercase, taking into account the specified locale.

var uppercased: String

An uppercase representation of the string.

var localizedUppercase: String

Returns a version of the string with all letters converted to uppercase, taking into account the current locale.

var capitalized: String

A capitalized representation of the string.

var localizedCapitalized: String

Returns a capitalized representation of the receiver using the current locale.

func capitalized(with: Locale?) -> String

Returns a capitalized representation of the receiver using the specified locale.

