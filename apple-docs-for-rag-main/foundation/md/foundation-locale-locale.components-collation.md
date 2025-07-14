

- Foundation
- Locale
- Locale.Components
-  collation 

Instance Property

# collation

The string sort order of the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var collation: Locale.Collation?
```

## Discussion

Set this property to override the locale’s default string sort order. To request the collation used by the locale, use the Locale property collation.

This property corresponds to the `co` key of the Unicode BCP 47 extension.

## See Also

### Specifying ordering components

struct Collation

A type that represents the string sort order used by the locale.

