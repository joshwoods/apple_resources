

- HealthKit
- HKAnchoredObjectQueryDescriptor
- HKAnchoredObjectQueryDescriptor.Result
-  newAnchor 

Instance Property

# newAnchor

A value corresponding to the last sample that the anchor query has returned.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
let newAnchor: HKQueryAnchor
```

## Discussion

Subsequent anchor object queries can use this anchor to receive only the samples saved and objects deleted after this query completed.

## See Also

### Accessing the Results

let addedSamples: [Sample]

An array containing the matching samples added to the HealthKit store.

let deletedObjects: [HKDeletedObject]

An array of objects deleted from the HealthKit store.

