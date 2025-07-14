

- SwiftUI
- SectionedFetchRequest
- SectionedFetchRequest.Configuration
-  sortDescriptors 

Instance Property

# sortDescriptors

The request’s sort descriptors, accessed as value types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var sortDescriptors: [SortDescriptor] { get set }
```

Available when `SectionIdentifier` conforms to `Hashable` and `Result` inherits `NSManagedObject`.

## Discussion

Set this configuration value to cause a SectionedFetchRequest to execute a fetch with a new collection of SortDescriptor instances. If you want to use NSSortDescriptor instances, set nsSortDescriptors instead. Use care to coordinate section and sort updates, as described in SectionedFetchRequest.Configuration.

Access this value for a given request by using the sortDescriptors property on the associated SectionedFetchResults instance, either directly or with a Binding.

## See Also

### Setting sort descriptors

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

