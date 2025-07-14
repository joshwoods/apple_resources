

- SwiftUI
- FetchedResults
-  sortDescriptors 

Instance Property

# sortDescriptors

The request’s sort descriptors, accessed as value types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var sortDescriptors: [SortDescriptor] { get nonmutating set }
```

Available when `Result` inherits `NSManagedObject`.

## Discussion

Set this value to cause the associated FetchRequest to execute a fetch with a new collection of SortDescriptor instances. The order of entities stored in the results collection may change as a result.

If you want to use NSSortDescriptor instances, set nsSortDescriptors instead.

## See Also

### Configuring the associated fetch request

var nsPredicate: NSPredicate?

The request’s predicate.

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

