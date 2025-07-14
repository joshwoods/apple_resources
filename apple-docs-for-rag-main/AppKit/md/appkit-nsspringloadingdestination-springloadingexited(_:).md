

- AppKit
- NSSpringLoadingDestination
-  springLoadingExited(\_:) 

Instance Method

# springLoadingExited(\_:)

Responds when a drag exits the bounds of the spring-loading destination.

macOS 10.11+

``` source
@MainActor
optional func springLoadingExited(_ draggingInfo: any NSDraggingInfo)
```

## Parameters 

`draggingInfo`  

An object of type `NSDraggingInfo`, which provides information about the drag event, including the dragged data.

## Discussion

This method is called when a drag exits the bounds of a spring-loaded destination.

This is a good place to clean up any initialization work that may have been performed during springLoadingEntered(_:).

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

func draggingEnded(any NSDraggingInfo)

Responds to the end of a drag operation.

