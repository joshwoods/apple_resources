

- AppKit
- NSObjectController
-  fetch(\_:) 

Instance Method

# fetch(\_:)

Causes the receiver to fetch the data objects specified by the entity name and fetch predicate.

macOS

``` source
@IBAction @MainActor
func fetch(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

## Discussion

Beginning with OS X v10.4 the result of this method is deferred until the next iteration of the runloop so that the error presentation mechanism can provide feedback as a sheet.

## See Also

### Core Data support

var entityName: String?

The entity name used by the receiver to create new objects.

var usesLazyFetching: Bool

A Boolean that indicates whether the receiver uses lazy fetching.

func defaultFetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns the default fetch request used by the receiver.

var fetchPredicate: NSPredicate?

The receiver’s fetch predicate.

var managedObjectContext: NSManagedObjectContext?

The receiver’s managed object context.

func fetch(with: NSFetchRequest&lt;any NSFetchRequestResult>?, merge: Bool) throws

Subclasses should override this method to customize a fetch request, for example to specify fetch limits.

