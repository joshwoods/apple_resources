

- UIKit
-  UIDragSession 

Protocol

# UIDragSession

The interface for configuring a drag session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIDragSession : UIDragDropSession
```

## Mentioned in 

Making a view into a drag source

## Topics

### Accessing local information

var localContext: Any?

The optional custom data that you attach to a drag session, visible only to the app in which the drag activity begins.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIDragDropSession

## See Also

### Drag sources

class UIDragItem

A representation of an underlying data item as a person drags it from one location to another.

protocol UIDragDropSession

The common interface for querying the state of both drag sessions and drop sessions.

protocol UIDragAnimating

The interface for providing custom animation alongside the system’s lift, drop, and cancellation animations.

