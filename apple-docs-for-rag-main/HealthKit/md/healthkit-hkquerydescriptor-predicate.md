

- HealthKit
- HKQueryDescriptor
-  predicate 

Instance Property

# predicate

The predicate that filters samples matching this descriptor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
@NSCopying
var predicate: NSPredicate? { get }
```

## Discussion

If the predicate is `nil`, the descriptor matches all samples of the data type specified by the sampleType property.

## See Also

### Accessing Descriptor Data

var sampleType: HKSampleType

The data type of samples that match this descriptor.

