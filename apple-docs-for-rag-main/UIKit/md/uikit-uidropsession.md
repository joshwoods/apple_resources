

- UIKit
-  UIDropSession 

Protocol

# UIDropSession

The interface for querying a drop session about its state and associated drag items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIDropSession : ProgressReporting, UIDragDropSession
```

## Mentioned in 

Making a view into a drop destination

## Topics

### Getting the drag session

var localDragSession: (any UIDragSession)?

The drag session that corresponds to this drop session, for in-app drag activities.

**Required**

### Loading objects

func loadObjects(ofClass: any NSItemProviderReading.Type, completion: ([any NSItemProviderReading]) -> Void) -> Progress

Creates and loads a new instance of the specified class for each drag item in the session.

**Required** Default implementation provided.

### Showing a progress indicator

var progressIndicatorStyle: UIDropSessionProgressIndicatorStyle

The drop-progress indicator style associated with the drop session.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- ProgressReporting
- UIDragDropSession

## See Also

### Drop destinations

class UIDropProposal

A configuration for the behavior of a drop interaction, required if a view accepts drop activities.

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

enum UIDropSessionProgressIndicatorStyle

The drop-progress indicator styles for the drop session, used while data is moving from the source to the destination.

