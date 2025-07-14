

- Core Data
- NSFetchedResultsController
-  fetchRequest 

Instance Property

# fetchRequest

The fetch request used to do the fetching.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fetchRequest: NSFetchRequest { get }
```

## Discussion

If you want to modify the fetch request, you must follow the steps described in Modifying the fetch request.

## See Also

### Related Documentation

init(fetchRequest: NSFetchRequest&lt;ResultType>, managedObjectContext: NSManagedObjectContext, sectionNameKeyPath: String?, cacheName: String?)

Returns a fetch request controller initialized using the given arguments.

### Getting Configuration Information

var managedObjectContext: NSManagedObjectContext

The managed object context used to fetch objects.

var sectionNameKeyPath: String?

The key path of the attribute that determines which section the fetched entity belongs to.

var cacheName: String?

The name of the file used to cache section information.

var delegate: (any NSFetchedResultsControllerDelegate)?

The object that is notified when the fetched results changed.

class func deleteCache(withName: String?)

Deletes the cached section information with the given name.

