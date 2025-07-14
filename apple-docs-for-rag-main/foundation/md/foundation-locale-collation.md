

- Foundation
- Locale
-  collation 

Instance Property

# collation

The string sort order of the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var collation: Locale.Collation { get }
```

## Discussion

This property corresponds to the `co` key of the Unicode BCP 47 extension.

For locale instances created with the `co` specifier (such as `en-US@co=phonetic`), or with a custom Locale.Components, this property represents the custom collation. Otherwise, it represents the locale’s default sort order.

## See Also

### Getting ordering components

struct Collation

A type that represents the string sort order used by the locale.

