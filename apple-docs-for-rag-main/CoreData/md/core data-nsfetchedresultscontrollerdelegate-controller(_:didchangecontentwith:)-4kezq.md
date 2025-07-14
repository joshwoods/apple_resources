

- Core Data
- NSFetchedResultsControllerDelegate
-  controller(\_:didChangeContentWith:) 

Instance Method

# controller(\_:didChangeContentWith:)

Notifies the receiver about changes to the content in the fetched results controller, by using a diffable data source snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func controller(
    _ controller: NSFetchedResultsController,
    didChangeContentWith snapshot: NSDiffableDataSourceSnapshot
)
```

## Discussion

To apply the changes, call applySnapshot(_:animatingDifferences:) on the collection or table view’s data source.

If this method is implemented, no other delegate methods are invoked.

## See Also

### Responding to Changes

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChangeContentWith: CollectionDifference&lt;NSManagedObjectID>)

Notifies the receiver about changes to the content in the fetched results controller, by using a collection difference.

func controllerWillChangeContent(NSFetchedResultsController&lt;any NSFetchRequestResult>)

Notifies the receiver that the fetched results controller is about to start processing of one or more changes due to an add, remove, move, or update.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChange: Any, at: IndexPath?, for: NSFetchedResultsChangeType, newIndexPath: IndexPath?)

Notifies the receiver that a fetched object has been changed due to an add, remove, move, or update.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChange: any NSFetchedResultsSectionInfo, atSectionIndex: Int, for: NSFetchedResultsChangeType)

Notifies the receiver of the addition or removal of a section.

func controllerDidChangeContent(NSFetchedResultsController&lt;any NSFetchRequestResult>)

Notifies the receiver that the fetched results controller has completed processing of one or more changes due to an add, remove, move, or update.

