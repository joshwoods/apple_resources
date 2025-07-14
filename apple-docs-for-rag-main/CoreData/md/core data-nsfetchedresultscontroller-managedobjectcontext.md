

- Core Data
- NSFetchedResultsController
-  managedObjectContext 

Instance Property

# managedObjectContext

The managed object context used to fetch objects.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var managedObjectContext: NSManagedObjectContext { get }
```

## Discussion

The controller registers to listen to change notifications on this context and properly update its result set and section information.

## See Also

### Getting Configuration Information

var fetchRequest: NSFetchRequest&lt;ResultType>

The fetch request used to do the fetching.

var sectionNameKeyPath: String?

The key path of the attribute that determines which section the fetched entity belongs to.

var cacheName: String?

The name of the file used to cache section information.

var delegate: (any NSFetchedResultsControllerDelegate)?

The object that is notified when the fetched results changed.

class func deleteCache(withName: String?)

Deletes the cached section information with the given name.

