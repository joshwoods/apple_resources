

- Core Data
- NSFetchedResultsController
-  cacheName 

Instance Property

# cacheName

The name of the file used to cache section information.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var cacheName: String? { get }
```

## Discussion

The file itself is stored in a private directory; you can only access it by name using deleteCache(withName:)

## See Also

### Related Documentation

init(fetchRequest: NSFetchRequest&lt;ResultType>, managedObjectContext: NSManagedObjectContext, sectionNameKeyPath: String?, cacheName: String?)

Returns a fetch request controller initialized using the given arguments.

### Getting Configuration Information

var fetchRequest: NSFetchRequest&lt;ResultType>

The fetch request used to do the fetching.

var managedObjectContext: NSManagedObjectContext

The managed object context used to fetch objects.

var sectionNameKeyPath: String?

The key path of the attribute that determines which section the fetched entity belongs to.

var delegate: (any NSFetchedResultsControllerDelegate)?

The object that is notified when the fetched results changed.

class func deleteCache(withName: String?)

Deletes the cached section information with the given name.

