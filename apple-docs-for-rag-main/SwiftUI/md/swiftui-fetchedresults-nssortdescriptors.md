

- SwiftUI
- FetchedResults
-  nsSortDescriptors 

Instance Property

# nsSortDescriptors

The request’s sort descriptors, accessed as reference types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var nsSortDescriptors: [NSSortDescriptor] { get nonmutating set }
```

## Discussion

Set this value to cause the associated FetchRequest to execute a fetch with a new collection of NSSortDescriptor instances. The order of managed objects stored in the results collection may change as a result.

If you want to use SortDescriptor instances, set sortDescriptors instead.

## See Also

### Configuring the associated fetch request

var nsPredicate: NSPredicate?

The request’s predicate.

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

