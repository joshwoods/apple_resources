

- Core Data
- NSFetchedResultsController
-  deleteCache(withName:) 

Type Method

# deleteCache(withName:)

Deletes the cached section information with the given name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func deleteCache(withName name: String?)
```

## Parameters 

`name`  

The name of the cache file to delete.

If `name` is `nil`, deletes all cache files.

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

var delegate: (any NSFetchedResultsControllerDelegate)?

The object that is notified when the fetched results changed.

