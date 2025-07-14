

- HealthKit
- HKHealthStore
-  earliestPermittedSampleDate() 

Instance Method

# earliestPermittedSampleDate()

Returns the earliest date permitted for samples.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func earliestPermittedSampleDate() -> Date
```

## Return Value

The earliest date that samples can use. You cannot save or query samples prior to this date.

## Mentioned in 

About the HealthKit framework

## Discussion

Attempts to save samples earlier than this date fail with an HKError.Code.errorInvalidArgument error. Attempts to query samples before this date return samples after this date.

## See Also

### Working with HealthKit objects

func delete(HKObject, withCompletion: (Bool, (any Error)?) -> Void)

Deletes the specified object from the HealthKit store.

func delete([HKObject], withCompletion: (Bool, (any Error)?) -> Void)

Deletes the specified objects from the HealthKit store.

func deleteObjects(of: HKObjectType, predicate: NSPredicate, withCompletion: (Bool, Int, (any Error)?) -> Void)

Deletes objects saved by this application that match the provided type and predicate.

func save(HKObject, withCompletion: (Bool, (any Error)?) -> Void)

Saves the provided object to the HealthKit store.

func save([HKObject], withCompletion: (Bool, (any Error)?) -> Void)

Saves an array of objects to the HealthKit store.

