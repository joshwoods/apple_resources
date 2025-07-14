

- HealthKit
- HKHealthStore
-  save(\_:withCompletion:) 

Instance Method

# save(\_:withCompletion:)

Saves an array of objects to the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func save(
    _ objects: [HKObject],
    withCompletion completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func save(_ objects: [HKObject]) async throws
```

## Parameters 

`objects`  

An array containing concrete subclasses of the HKObject class (any of the HKCategorySample, HKQuantitySample, HKCorrelation, or HKWorkout classes).

`completion`  

A block that this method calls as soon as the save operation is complete. This block is passed the following parameters:

success  
A Boolean value. This parameter contains true if the objects were successfully saved to the HealthKit store; otherwise, false.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Discussion

This method operates asynchronously. As soon as the save operation is finished, it calls the completion block on a background queue.

If your app has not requested permission to share the object’s data type, the method fails with an HKError.Code.errorAuthorizationNotDetermined error. If your app has been denied permission to save the object’s data type, it fails with an HKError.Code.errorAuthorizationDenied error. Saving an object with the same unique identifier as an object already in the HealthKit store fails with an HKError.Code.errorInvalidArgument error. When saving multiple objects, if any object cannot be saved, none of them are saved.

In iOS 9.0 and later, saving an object to the HealthKit store sets the object’s sourceRevision property to a HKSourceRevision instance representing the saving app. On earlier versions of iOS, saving an object sets the source property to a HKSource instance instead. In both cases, these values are available only after the object is retrieved from the HealthKit store. The original object is not changed.

All samples retrieved by iOS 9.0 and later are given a valid sourceRevision property. If the sample was saved using an earlier version of iOS, the source revision’s version is set to `nil`.

## See Also

### Working with HealthKit objects

func delete(HKObject, withCompletion: (Bool, (any Error)?) -> Void)

Deletes the specified object from the HealthKit store.

func delete([HKObject], withCompletion: (Bool, (any Error)?) -> Void)

Deletes the specified objects from the HealthKit store.

func deleteObjects(of: HKObjectType, predicate: NSPredicate, withCompletion: (Bool, Int, (any Error)?) -> Void)

Deletes objects saved by this application that match the provided type and predicate.

func earliestPermittedSampleDate() -> Date

Returns the earliest date permitted for samples.

func save(HKObject, withCompletion: (Bool, (any Error)?) -> Void)

Saves the provided object to the HealthKit store.

