

- Foundation
- Locale
- Locale.Components
-  variant 

Instance Property

# variant

An optional variant used by the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var variant: Locale.Variant?
```

## Discussion

Set this property to override the variant of the locale.

This property corresponds to the `va` key of the Unicode BCP 47 extension.

## See Also

### Specifying region components

var region: Locale.Region?

The region used by the locale.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

var subdivision: Locale.Subdivision?

The optional subdivision of the region used by this locale.

struct Subdivision

A type that represents a subdivision of a region, such as a state in the US or a province in Canada.

struct Variant

A type that represents a locale’s languate variant.

