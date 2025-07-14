

- MapKit
- MKDistanceFormatter
-  locale 

Instance Property

# locale

The locale to use when formatting strings.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
var locale: Locale! { get set }
```

## Discussion

If you don’t specify an explicit locale, the formatter uses the user’s current locale information.

## See Also

### Specifying the format

var units: MKDistanceFormatter.Units

The measuring system — imperial or metric — to use for units.

enum Units

Constants that reflect the type of units to use in the string.

var unitStyle: MKDistanceFormatter.DistanceUnitStyle

The preferred style for units.

enum DistanceUnitStyle

Constants that indicate the format style to use for strings.

