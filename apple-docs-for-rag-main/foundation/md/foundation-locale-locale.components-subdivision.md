

- Foundation
- Locale
- Locale.Components
-  subdivision 

Instance Property

# subdivision

The optional subdivision of the region used by this locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var subdivision: Locale.Subdivision?
```

## Discussion

Set this property to override the locale’s regional subdivision of region.

This property corresponds to the `sd` key of the Unicode BCP 47 extension.

## See Also

### Specifying region components

var region: Locale.Region?

The region used by the locale.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

struct Subdivision

A type that represents a subdivision of a region, such as a state in the US or a province in Canada.

var variant: Locale.Variant?

An optional variant used by the locale.

struct Variant

A type that represents a locale’s languate variant.

