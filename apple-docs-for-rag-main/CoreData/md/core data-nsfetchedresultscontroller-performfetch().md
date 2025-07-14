

- Core Data
- NSFetchedResultsController
-  performFetch() 

Instance Method

# performFetch()

Executes the controller’s fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func performFetch() throws
```

## Discussion

After you execute this method, access the controller’s fetched objects using the fetchedObjects property.

Important

If you specify a value for the `sectionNameKeyPath` parameter when you initialize the fetched results controller, the fetch request must include a sort descriptor for the corresponding key path; otherwise, the fetch fails.

## See Also

### Initializing a Fetched Results Controller

init(fetchRequest: NSFetchRequest&lt;ResultType>, managedObjectContext: NSManagedObjectContext, sectionNameKeyPath: String?, cacheName: String?)

Returns a fetch request controller initialized using the given arguments.

