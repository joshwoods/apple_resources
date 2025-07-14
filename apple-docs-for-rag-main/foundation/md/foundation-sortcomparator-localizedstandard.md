

- Foundation
- SortComparator
-  localizedStandard 

Type Property

# localizedStandard

A comparator that compares a string using a localized, numeric comparison in the current locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var localizedStandard: String.Comparator { get }
```

Available when `Self` is `String.Comparator`.

## Discussion

Compares String in a manner similar to the Finder.

## See Also

### Inspecting a Comparator

var order: SortOrder

The sort order that the comparator uses to compare.

**Required**

static var localized: String.Comparator

A comparator that compares a string using a localized comparison in the current locale.

