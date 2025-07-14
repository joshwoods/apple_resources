

- HealthKit
- HKAnchoredObjectQueryDescriptor
- HKAnchoredObjectQueryDescriptor.Result
-  deletedObjects 

Instance Property

# deletedObjects

An array of objects deleted from the HealthKit store.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
let deletedObjects: [HKDeletedObject]
```

## See Also

### Accessing the Results

let addedSamples: [Sample]

An array containing the matching samples added to the HealthKit store.

let newAnchor: HKQueryAnchor

A value corresponding to the last sample that the anchor query has returned.

