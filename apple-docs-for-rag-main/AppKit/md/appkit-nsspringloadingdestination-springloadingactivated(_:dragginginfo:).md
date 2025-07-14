

- AppKit
- NSSpringLoadingDestination
-  springLoadingActivated(\_:draggingInfo:) 

Instance Method

# springLoadingActivated(\_:draggingInfo:)

Responds to the activation or deactivation of spring-loading on a destination.

macOS 10.11+

``` source
@MainActor
func springLoadingActivated(
    _ activated: Bool,
    draggingInfo: any NSDraggingInfo
)
```

**Required**

## Parameters 

`activated`  

A Boolean value indicating whether spring-loading has been activated on the destination. true indicates that spring-loading has been activated. false indicates that spring-loading has been deactivated.

`draggingInfo`  

An `NSDraggingInfo` object, which provides information about the drag event, including the dragged data.

## Discussion

Typically, spring-loading is fully activated when a hover timeout occurs or the user finishes force clicking on a destination object to initiate spring-loading. In these cases, the `springLoadingActivated:draggingInfo:` method is only called once with an `activated` parameter value of true.

However, if the destination is configured with continuous activation (`NSSpringLoadingOptions` was set to `NSSpringLoadingContinuousActivation`), then the `springLoadingActivated:draggingInfo:` method is called twice. First, it’s called with an `activated` parameter value of true when a hover timeout occurs or the user begins force clicking on a destination object to initiate spring-loading. Then, it’s called again with an `activated` parameter value of false when the hover exits the destination’s bounds or the user finishes force clicking on the destination object.

## See Also

### Related Documentation

Drag and Drop Programming Topics

struct NSSpringLoadingOptions

These constants denote the type of spring-loading behavior configured for the destination object.

protocol NSDraggingInfo

A set of methods that supply information about a dragging session.

### Respond to Spring-loading Events

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

