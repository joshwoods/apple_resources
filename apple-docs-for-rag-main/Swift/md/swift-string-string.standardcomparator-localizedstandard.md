

- Swift
- String
- String.StandardComparator
-  localizedStandard 

Type Property

# localizedStandard

Compares `String`s as compared by the Finder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let localizedStandard: String.StandardComparator
```

## Discussion

Uses a localized, numeric comparison in the current locale.

The default `SortComparator` used in `String` comparisons.

