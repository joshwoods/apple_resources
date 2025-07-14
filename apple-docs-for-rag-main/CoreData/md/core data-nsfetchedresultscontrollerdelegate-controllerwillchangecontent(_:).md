

- Core Data
- NSFetchedResultsControllerDelegate
-  controllerWillChangeContent(\_:) 

Instance Method

# controllerWillChangeContent(\_:)

Notifies the receiver that the fetched results controller is about to start processing of one or more changes due to an add, remove, move, or update.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
optional func controllerWillChangeContent(_ controller: NSFetchedResultsController)
```

## Parameters 

`controller`  

The fetched results controller that sent the message.

## Discussion

This method is invoked before all invocations of controller(_:didChange:at:for:newIndexPath:) and controller(_:didChange:atSectionIndex:for:) have been sent for a given change event (such as the controller receiving a NSManagedObjectContextDidSave notification).

## See Also

### Related Documentation

Core Data Programming Guide

### Responding to Changes

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChangeContentWith: NSDiffableDataSourceSnapshot)

Notifies the receiver about changes to the content in the fetched results controller, by using a diffable data source snapshot.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChangeContentWith: CollectionDifference&lt;NSManagedObjectID>)

Notifies the receiver about changes to the content in the fetched results controller, by using a collection difference.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChange: Any, at: IndexPath?, for: NSFetchedResultsChangeType, newIndexPath: IndexPath?)

Notifies the receiver that a fetched object has been changed due to an add, remove, move, or update.

func controller(NSFetchedResultsController&lt;any NSFetchRequestResult>, didChange: any NSFetchedResultsSectionInfo, atSectionIndex: Int, for: NSFetchedResultsChangeType)

Notifies the receiver of the addition or removal of a section.

func controllerDidChangeContent(NSFetchedResultsController&lt;any NSFetchRequestResult>)

Notifies the receiver that the fetched results controller has completed processing of one or more changes due to an add, remove, move, or update.

