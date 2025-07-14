

- AppKit
- NSObjectController
-  usesLazyFetching 

Instance Property

# usesLazyFetching

A Boolean that indicates whether the receiver uses lazy fetching.

macOS 10.5+

``` source
var usesLazyFetching: Bool { get set }
```

## Discussion

When enabled the controller uses a number of techniques that typically make managing large data sets more efficient. As with all optimizations, you should use suitable performance analysis tools (such as Instruments) to determine the best solution.

## See Also

### Core Data support

var entityName: String?

The entity name used by the receiver to create new objects.

func fetch(Any?)

Causes the receiver to fetch the data objects specified by the entity name and fetch predicate.

func defaultFetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns the default fetch request used by the receiver.

var fetchPredicate: NSPredicate?

The receiver’s fetch predicate.

var managedObjectContext: NSManagedObjectContext?

The receiver’s managed object context.

func fetch(with: NSFetchRequest&lt;any NSFetchRequestResult>?, merge: Bool) throws

Subclasses should override this method to customize a fetch request, for example to specify fetch limits.

