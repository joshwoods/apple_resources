

- Core Data
- NSFetchedResultsControllerDelegate
-  controller(\_:didChange:atSectionIndex:for:) 

Instance Method

# controller(\_:didChange:atSectionIndex:for:)

Notifies the receiver of the addition or removal of a section.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
optional func controller(
    _ controller: NSFetchedResultsController,
    didChange sectionInfo: any NSFetchedResultsSectionInfo,
    atSectionIndex sectionIndex: Int,
    for type: NSFetchedResultsChangeType
)
```

## Parameters 

`controller`  

The fetched results controller that sent the message.

`sectionInfo`  

The section that changed.

`sectionIndex`  

The index of the changed section.

`type`  

The type of change (insert or delete). Valid values are NSFetchedResultsChangeType.insert and NSFetchedResultsChangeType.delete.

## Discussion

The fetched results controller reports changes to its section before changes to the fetched result objects.

### Special Considerations

This method may be invoked many times during an update event (for example, if you are importing data on a background thread and adding them to the context in a batch). You should consider carefully whether you want to update the table view on receipt of each message.

## See Also

### Responding to Changes

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChangeContentWith: NSDiffableDataSourceSnapshot)

Notifies the receiver about changes to the content in the fetched results controller, by using a diffable data source snapshot.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChangeContentWith: CollectionDifference&lt;NSManagedObjectID>)

Notifies the receiver about changes to the content in the fetched results controller, by using a collection difference.

func controllerWillChangeContent(NSFetchedResultsController&lt;any NSFetchRequestResult>)

Notifies the receiver that the fetched results controller is about to start processing of one or more changes due to an add, remove, move, or update.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChange: Any, at: IndexPath?, for: NSFetchedResultsChangeType, newIndexPath: IndexPath?)

Notifies the receiver that a fetched object has been changed due to an add, remove, move, or update.

func controllerDidChangeContent(NSFetchedResultsController&lt;any NSFetchRequestResult>)

Notifies the receiver that the fetched results controller has completed processing of one or more changes due to an add, remove, move, or update.

