

- Foundation
- Calendar
-  eraSymbols 

Instance Property

# eraSymbols

A list of eras in this calendar, localized to the Calendar’s `locale`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var eraSymbols: [String] { get }
```

## Discussion

For example, for English in the Gregorian calendar, returns `["BC", "AD"]`.

Note

By default, Calendars have no locale set. If you wish to receive a localized answer, be sure to set the `locale` property first - most likely to `Locale.autoupdatingCurrent`.

## See Also

### Getting Era Symbols

var longEraSymbols: [String]

A list of longer-named eras in this calendar, localized to the Calendar’s `locale`.

