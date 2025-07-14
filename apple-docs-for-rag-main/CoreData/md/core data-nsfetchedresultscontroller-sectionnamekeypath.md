

- Core Data
- NSFetchedResultsController
-  sectionNameKeyPath 

Instance Property

# sectionNameKeyPath

The key path of the attribute that determines which section the fetched entity belongs to.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sectionNameKeyPath: String? { get }
```

## Discussion

This property returns the value you specify for the `sectionNameKeyPath` parameter when you initialize the fetched results controller.

If the controller generates sections, typically this property’s value matches the specified key path of the first sort descriptor in the controller’s fetch request. If the two key paths don’t match, then they must generate the same relative ordering. For example, the fetch request’s first sort descriptor might specify the key path of a persistent attribute, but sectionNameKeyPath might specify the key path of a transient attribute that derives its value from the persistent one.

## See Also

### Getting Configuration Information

var fetchRequest: NSFetchRequest&lt;ResultType>

The fetch request used to do the fetching.

var managedObjectContext: NSManagedObjectContext

The managed object context used to fetch objects.

var cacheName: String?

The name of the file used to cache section information.

var delegate: (any NSFetchedResultsControllerDelegate)?

The object that is notified when the fetched results changed.

class func deleteCache(withName: String?)

Deletes the cached section information with the given name.

