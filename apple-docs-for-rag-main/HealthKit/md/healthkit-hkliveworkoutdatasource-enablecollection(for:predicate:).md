

- HealthKit
- HKLiveWorkoutDataSource
-  enableCollection(for:predicate:) 

Instance Method

# enableCollection(for:predicate:)

Begins automatically calculating statistics for samples that match the quantity type and predicate.

macOSwatchOS 5.0+

``` source
func enableCollection(
    for quantityType: HKQuantityType,
    predicate: NSPredicate?
)
```

## Mentioned in 

Dividing a HealthKit workout into activities

## See Also

### Calculating statistics

func disableCollection(for: HKQuantityType)

Stops automatically calculating statistics for the quantity type.

