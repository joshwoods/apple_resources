

- AppKit
- NSObjectController
-  fetchPredicate 

Instance Property

# fetchPredicate

The receiver’s fetch predicate.

macOS

``` source
var fetchPredicate: NSPredicate? { get set }
```

## Discussion

The receiver uses `predicate` when fetching its content, for example in fetch(_:). If you need to customize the fetching behavior further, you can override fetch(with:merge:).

## See Also

### Core Data support

var entityName: String?

The entity name used by the receiver to create new objects.

func fetch(Any?)

Causes the receiver to fetch the data objects specified by the entity name and fetch predicate.

var usesLazyFetching: Bool

A Boolean that indicates whether the receiver uses lazy fetching.

func defaultFetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns the default fetch request used by the receiver.

var managedObjectContext: NSManagedObjectContext?

The receiver’s managed object context.

func fetch(with: NSFetchRequest&lt;any NSFetchRequestResult>?, merge: Bool) throws

Subclasses should override this method to customize a fetch request, for example to specify fetch limits.

