

- SwiftUI
- SectionedFetchRequest
- SectionedFetchRequest.Configuration
-  nsSortDescriptors 

Instance Property

# nsSortDescriptors

The request’s sort descriptors, accessed as reference types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var nsSortDescriptors: [NSSortDescriptor]
```

## Discussion

Set this configuration value to cause a SectionedFetchRequest to execute a fetch with a new collection of NSSortDescriptor instances. If you want to use SortDescriptor instances, set sortDescriptors instead. Use care to coordinate section and sort updates, as described in SectionedFetchRequest.Configuration.

Access this value for a given request by using the nsSortDescriptors property on the associated SectionedFetchResults instance, either directly or with a Binding.

## See Also

### Setting sort descriptors

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

