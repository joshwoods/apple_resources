

- AppKit
- NSSpringLoadingDestination
-  springLoadingUpdated(\_:) 

Instance Method

# springLoadingUpdated(\_:)

Returns whether to enable or disable spring-loading as a drag moves within the bounds of the spring-loading destination or `draggingInfo` changes during the drag.

macOS 10.11+

``` source
@MainActor
optional func springLoadingUpdated(_ draggingInfo: any NSDraggingInfo) -> NSSpringLoadingOptions
```

## Parameters 

`draggingInfo`  

An object of type `NSDraggingInfo`, which provides information about the drag event, including the dragged data.

## Return Value

A value of type `NSSpringLoadingOptions` to enable or disable spring-loading. A value of `NSSpringLoadingEnabled` enables typical spring-loading behavior.

## Discussion

This method is called periodically as a drag changes position within the bounds of a spring-loaded destination or the `draggingInfo` changes during the drag. It returns a value of type `NSSpringLoadingOptions` to enable or disable spring-loading for the destination. If this method is not implemented, then spring-loading is enabled or disabled for the destination based on the return value of the `springLoadingEntered:` method.

Note that you *must* implement either this method or springLoadingEntered(_:) to enable spring-loading.

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

func springLoadingExited(any NSDraggingInfo)

Responds when a drag exits the bounds of the spring-loading destination.

func draggingEnded(any NSDraggingInfo)

Responds to the end of a drag operation.

