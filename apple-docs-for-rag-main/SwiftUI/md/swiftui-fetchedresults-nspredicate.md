

- SwiftUI
- FetchedResults
-  nsPredicate 

Instance Property

# nsPredicate

The request’s predicate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var nsPredicate: NSPredicate? { get nonmutating set }
```

## Discussion

Set this value to cause the associated FetchRequest to execute a fetch with a new predicate, producing an updated collection of results.

## See Also

### Configuring the associated fetch request

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

