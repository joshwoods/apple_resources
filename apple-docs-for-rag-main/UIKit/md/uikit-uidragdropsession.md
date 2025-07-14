

- UIKit
-  UIDragDropSession 

Protocol

# UIDragDropSession

The common interface for querying the state of both drag sessions and drop sessions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIDragDropSession : NSObjectProtocol
```

## Topics

### Checking for drag items

func canLoadObjects(ofClass: any NSItemProviderReading.Type) -> Bool

Returns a Boolean value that indicates whether at least one drag item in the session can create an instance of the specified class.

**Required** Default implementation provided.

func hasItemsConforming(toTypeIdentifiers: [String]) -> Bool

Returns a Boolean value that indicates whether at least one drag item in the session conforms to at least one of the specified UTIs.

**Required**

var items: [UIDragItem]

An array of drag items in the drag session or drop session.

**Required**

### Checking for drag and drop session restrictions

var allowsMoveOperation: Bool

A Boolean value that indicates whether the drag session permits moving drag items within the same app.

**Required**

var isRestrictedToDraggingApplication: Bool

A Boolean value that indicates whether the drag session is confined to the app that started the drag activity.

**Required**

### Getting the location of a drag activity

func location(in: UIView) -> CGPoint

Returns the geometrical location of the user’s drag activity within the specified view.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIDragSession
- UIDropSession

## See Also

### Drag sources

class UIDragItem

A representation of an underlying data item as a person drags it from one location to another.

protocol UIDragSession

The interface for configuring a drag session.

protocol UIDragAnimating

The interface for providing custom animation alongside the system’s lift, drop, and cancellation animations.

