

- Core Data
- NSFetchedResultsControllerDelegate
-  controller(\_:didChange:at:for:newIndexPath:) 

Instance Method

# controller(\_:didChange:at:for:newIndexPath:)

Notifies the receiver that a fetched object has been changed due to an add, remove, move, or update.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func controller(
    _ controller: NSFetchedResultsController,
    didChange anObject: Any,
    at indexPath: IndexPath?,
    for type: NSFetchedResultsChangeType,
    newIndexPath: IndexPath?
)
```

## Parameters 

`controller`  

The fetched results controller that sent the message.

`anObject`  

The object in controller’s fetched results that changed.

`indexPath`  

The index path of the changed object (this value is `nil` for insertions).

`type`  

The type of change. For valid values see NSFetchedResultsChangeType.

`newIndexPath`  

The destination path for the object for insertions or moves (this value is `nil` for a deletion).

## Discussion

The fetched results controller reports changes to its section before changes to the fetch result objects.

Changes are reported with the following heuristics:

- On add and remove operations, only the added/removed object is reported.

It’s assumed that all objects that come after the affected object are also moved, but these moves are not reported. 

- A move is reported when the changed attribute on the object is one of the sort descriptors used in the fetch request.

An update of the object is assumed in this case, but no separate update message is sent to the delegate.

- An update is reported when an object’s state changes, but the changed attributes aren’t part of the sort keys. 

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

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChange: any NSFetchedResultsSectionInfo, atSectionIndex: Int, for: NSFetchedResultsChangeType)

Notifies the receiver of the addition or removal of a section.

func controllerDidChangeContent(NSFetchedResultsController&lt;any NSFetchRequestResult>)

Notifies the receiver that the fetched results controller has completed processing of one or more changes due to an add, remove, move, or update.

