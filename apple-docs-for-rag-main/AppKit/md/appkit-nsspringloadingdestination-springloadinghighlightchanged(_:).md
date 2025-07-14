

- AppKit
- NSSpringLoadingDestination
-  springLoadingHighlightChanged(\_:) 

Instance Method

# springLoadingHighlightChanged(\_:)

Updates the destination’s user interface to display a new highlighting style during a spring-loading operation.

macOS 10.11+

``` source
@MainActor
func springLoadingHighlightChanged(_ draggingInfo: any NSDraggingInfo)
```

**Required**

## Parameters 

`draggingInfo`  

An object of type `NSDraggingInfo`, which provides information about the drag event, including a highlighting style to apply.

## Discussion

During a spring-loaded operation, a destination may initiate animated highlighting to visually cue the user that spring-loading has been engaged or disengaged. This method is called as different stages of this animation are reached, providing an opportunity to change the highlighting style. Check the `springLoadingHighlight` property of the `draggingInfo` object to determine the style of highlighting to apply. Then, update the destination’s user interface accordingly.

Important

Do not use highlighting as a means to determine whether spring-loading has actually been activated or deactivated. The springLoadingActivated(_:draggingInfo:) method alerts your app when spring-loading activation occurs.

## See Also

### Related Documentation

struct NSDragOperation

A group of constants that represent which operations the dragging source can perform on dragging items.

struct NSSpringLoadingOptions

These constants denote the type of spring-loading behavior configured for the destination object.

protocol NSDraggingInfo

A set of methods that supply information about a dragging session.

### Respond to Spring-loading Events

func springLoadingActivated(Bool, draggingInfo: any NSDraggingInfo)

Responds to the activation or deactivation of spring-loading on a destination.

**Required**

func springLoadingEntered(any NSDraggingInfo) -> NSSpringLoadingOptions

Returns whether to enable or disable spring-loading when a drag enters the bounds of the spring-loading destination.

func springLoadingUpdated(any NSDraggingInfo) -> NSSpringLoadingOptions

Returns whether to enable or disable spring-loading as a drag moves within the bounds of the spring-loading destination or `draggingInfo` changes during the drag.

func springLoadingExited(any NSDraggingInfo)

Responds when a drag exits the bounds of the spring-loading destination.

func draggingEnded(any NSDraggingInfo)

Responds to the end of a drag operation.

