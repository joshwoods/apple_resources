

- Core Data
- NSFetchRequest
-  sortDescriptors 

Instance Property

# sortDescriptors

The sort descriptors of the fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sortDescriptors: [NSSortDescriptor]? { get set }
```

## Discussion

The sort descriptors specify how the objects returned when the NSFetchRequest is issued should be ordered—for example, by last name and then by first name. The sort descriptors are applied in the order in which they appear in the `sortDescriptors` array (serially in lowest-array-index-first order).

A value of `nil` is treated as no sort descriptors.

