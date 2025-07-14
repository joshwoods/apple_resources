

- Core Data
- NSFetchedResultsController
-  delegate 

Instance Property

# delegate

The object that is notified when the fetched results changed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var delegate: (any NSFetchedResultsControllerDelegate)? { get set }
```

## Discussion

If you do not specify a delegate, the controller does not track changes to managed objects associated with its managed object context.

## See Also

### Getting Configuration Information

var fetchRequest: NSFetchRequest&lt;ResultType>

The fetch request used to do the fetching.

var managedObjectContext: NSManagedObjectContext

The managed object context used to fetch objects.

var sectionNameKeyPath: String?

The key path of the attribute that determines which section the fetched entity belongs to.

var cacheName: String?

The name of the file used to cache section information.

class func deleteCache(withName: String?)

Deletes the cached section information with the given name.

