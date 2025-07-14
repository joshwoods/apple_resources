

- HealthKit
- HKQueryDescriptor
-  init(sampleType:predicate:) 

Initializer

# init(sampleType:predicate:)

Creates a new descriptor for the data type and predicate you provided.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    sampleType: HKSampleType,
    predicate: NSPredicate?
)
```

## Parameters 

`sampleType`  

The data type of samples that match this descriptor. For more information, see Data types.

`predicate`  

The predicate used to filter samples that match this descriptor. If the predicate is `nil`, the descriptor matches all samples of the specified data type.

