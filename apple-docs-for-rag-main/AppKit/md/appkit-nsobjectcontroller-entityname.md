

- AppKit
- NSObjectController
-  entityName 

Instance Property

# entityName

The entity name used by the receiver to create new objects.

macOS

``` source
var entityName: String? { get set }
```

## See Also

### Core Data support

func fetch(Any?)

Causes the receiver to fetch the data objects specified by the entity name and fetch predicate.

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

