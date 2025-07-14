

- AppKit
- NSSpringLoadingDestination
-  draggingEnded(\_:) 

Instance Method

# draggingEnded(\_:)

Responds to the end of a drag operation.

macOS 10.11+

``` source
@MainActor
optional func draggingEnded(_ draggingInfo: any NSDraggingInfo)
```

## Parameters 

`draggingInfo`  

An object of type `NSDraggingInfo`, which provides information about the drag event, including the dragged data.

## Discussion

This method is called when a drag operation has ended. If the destination object is both a dragging destination (class `NSDraggingDestination`) and a spring-loading destination (class `NSSpringLoadingDestination`), note that this method is only called once.

## See Also

### Related Documentation

struct NSSpringLoadingOptions

These constants denote the type of spring-loading behavior configured for the destination object.

protocol NSDraggingInfo

A set of methods that supply information about a dragging session.

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

