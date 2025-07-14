

- MapKit
- MKDistanceFormatter
-  unitStyle 

Instance Property

# unitStyle

The preferred style for units.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
var unitStyle: MKDistanceFormatter.DistanceUnitStyle { get set }
```

## Discussion

You can abbreviate or fully spell out units. The default value of this property is MKDistanceFormatter.DistanceUnitStyle.default, which bases the style on the user’s locale and language settings.

## See Also

### Specifying the format

var locale: Locale!

The locale to use when formatting strings.

var units: MKDistanceFormatter.Units

The measuring system — imperial or metric — to use for units.

enum Units

Constants that reflect the type of units to use in the string.

enum DistanceUnitStyle

Constants that indicate the format style to use for strings.

