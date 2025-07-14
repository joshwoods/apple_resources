

- Foundation
- SortComparator
-  localized 

Type Property

# localized

A comparator that compares a string using a localized comparison in the current locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var localized: String.Comparator { get }
```

Available when `Self` is `String.Comparator`.

## See Also

### Inspecting a Comparator

var order: SortOrder

The sort order that the comparator uses to compare.

**Required**

static var localizedStandard: String.Comparator

A comparator that compares a string using a localized, numeric comparison in the current locale.

