

- HealthKit
- HKQuantitySample
-  quantityType 

Instance Property

# quantityType

The quantity type for this sample.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var quantityType: HKQuantityType { get }
```

## Discussion

This property contains a reference to the sampleType property that is cast as an HKQuantityType object.

## See Also

### Getting Property Data

var quantity: HKQuantity

The quantity for this sample.

var count: Int

The number of quantities contained in this sample.

