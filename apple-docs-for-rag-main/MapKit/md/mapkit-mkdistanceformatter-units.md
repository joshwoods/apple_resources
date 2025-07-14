

- MapKit
- MKDistanceFormatter
-  units 

Instance Property

# units

The measuring system — imperial or metric — to use for units.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
var units: MKDistanceFormatter.Units { get set }
```

## Discussion

You can use this property to explicitly set the measuring system for units. The default value of this property is MKDistanceFormatter.Units.default, which bases the measuring system on the user’s locale.

## See Also

### Specifying the format

var locale: Locale!

The locale to use when formatting strings.

enum Units

Constants that reflect the type of units to use in the string.

var unitStyle: MKDistanceFormatter.DistanceUnitStyle

The preferred style for units.

enum DistanceUnitStyle

Constants that indicate the format style to use for strings.

