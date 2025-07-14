

- AppKit
-  NSSpringLoadingDestination 

Protocol

# NSSpringLoadingDestination

A set of methods that the destination object (or recipient) of a dragged object can implement to support spring-loading.

macOS

``` source
protocol NSSpringLoadingDestination : NSObjectProtocol
```

## Overview

Spring-loading is the act of dragging an object onto a destination object and hovering or force-clicking to activate the destination object A view can be configured as a drag-and-drop destination, a spring-loading destination, or both. If a view implements both drag-and-drop and spring-loading, then it will receive messages for both operations.

Note that the view beneath the cursor during a drag receives priority. For example, if a parent view implements drag-and-drop and a subview implements spring-loading, then the parent view will not receive drag-and-drop messages while the cursor is over the subview.

## Topics

### Respond to Spring-loading Events

func springLoadingActivated(Bool, draggingInfo: any NSDraggingInfo)

Responds to the activation or deactivation of spring-loading on a destination.

**Required**

func springLoadingHighlightChanged(any NSDraggingInfo)

Updates the destination’s user interface to display a new highlighting style during a spring-loading operation.

**Required**

func springLoadingEntered(any NSDraggingInfo) -> NSSpringLoadingOptions

Returns whether to enable or disable spring-loading when a drag enters the bounds of the spring-loading destination.

func springLoadingUpdated(any NSDraggingInfo) -> NSSpringLoadingOptions

Returns whether to enable or disable spring-loading as a drag moves within the bounds of the spring-loading destination or `draggingInfo` changes during the drag.

func springLoadingExited(any NSDraggingInfo)

Responds when a drag exits the bounds of the spring-loading destination.

func draggingEnded(any NSDraggingInfo)

Responds to the end of a drag operation.

### Constants

struct NSSpringLoadingOptions

These constants denote the type of spring-loading behavior configured for the destination object.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drop Targets

protocol NSDraggingDestination

A set of methods that the destination object (or recipient) of a dragged image must implement.

protocol NSDraggingInfo

A set of methods that supply information about a dragging session.

