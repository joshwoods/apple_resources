

- HealthKit
- HKHealthStore
-  deleteObjects(of:predicate:withCompletion:) 

Instance Method

# deleteObjects(of:predicate:withCompletion:)

Deletes objects saved by this application that match the provided type and predicate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func deleteObjects(
    of objectType: HKObjectType,
    predicate: NSPredicate,
    withCompletion completion: @escaping (Bool, Int, (any Error)?) -> Void
)
```

``` source
func deleteObjects(
    of objectType: HKObjectType,
    predicate: NSPredicate
) async throws -> Int
```

## Parameters 

`objectType`  

The type of object to be deleted.

`predicate`  

A predicate used to filter the objects to be deleted. This method only deletes objects that match the predicate.

`completion`  

A block that this method calls as soon as the delete operation is complete. This block is passed the following parameters:

success  
A Boolean value. This parameter contains true if the objects were successfully deleted; otherwise, false.

deletedObjectCount  
The number of objects deleted.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Discussion

Your app can delete only those objects that it has previously saved to the HealthKit store. If the user revokes sharing permission for an object type, you can no longer delete those objects. This method operates asynchronously. As soon as the delete operation is finished, it calls the completion block on a background queue.

If your app has not requested permission to share an object’s data type, the method fails with an HKError.Code.errorAuthorizationNotDetermined error. If your app has been denied permission to share an object’s data type, it fails with an HKError.Code.errorAuthorizationDenied error. When deleting multiple objects, if any object cannot be deleted, none of them are deleted.

HealthKit stores temporary HKDeletedObject entries, letting you query for recently deleted objects. However, the deleted objects are periodically removed to save storage space. If you want your app to receive notifications about all the deleted objects, set up an observer query, and enable it for background delivery. In the background query’s update handler, create an anchored object query to gather the list of recently deleted objects.

Note

Although your app can manage only the objects it created and saved, the users can always delete any data they want using the Health app.

## See Also

### Working with HealthKit objects

func delete(HKObject, withCompletion: (Bool, (any Error)?) -> Void)

Deletes the specified object from the HealthKit store.

func delete([HKObject], withCompletion: (Bool, (any Error)?) -> Void)

Deletes the specified objects from the HealthKit store.

func earliestPermittedSampleDate() -> Date

Returns the earliest date permitted for samples.

func save(HKObject, withCompletion: (Bool, (any Error)?) -> Void)

Saves the provided object to the HealthKit store.

func save([HKObject], withCompletion: (Bool, (any Error)?) -> Void)

Saves an array of objects to the HealthKit store.

