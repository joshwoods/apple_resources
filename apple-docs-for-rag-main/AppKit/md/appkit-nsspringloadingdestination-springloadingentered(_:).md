

- AppKit
- NSSpringLoadingDestination
-  springLoadingEntered(\_:) 

Instance Method

# springLoadingEntered(\_:)

Returns whether to enable or disable spring-loading when a drag enters the bounds of the spring-loading destination.

macOS 10.11+

``` source
@MainActor
optional func springLoadingEntered(_ draggingInfo: any NSDraggingInfo) -> NSSpringLoadingOptions
```

## Parameters 

`draggingInfo`  

An object of type `NSDraggingInfo`, which provides information about the drag event, including the dragged data.

## Return Value

A value of type `NSSpringLoadingOptions` to enable or disable spring-loading. Returning a value of `NSSpringLoadingEnabled` enables typical spring-loading behavior that is appropriate in most cases.

## Discussion

This method is called when a drag enters the bounds of the spring-loading destination. It returns a value of type `NSSpringLoadingOptions` to enable or disable spring-loading for the destination.

This method provides an opportunity to perform work in preparation for spring-loading becoming engaged.

Note that you *must* implement either this method or springLoadingUpdated(_:) to enable spring-loading.

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

func springLoadingUpdated(any NSDraggingInfo) -> NSSpringLoadingOptions

Returns whether to enable or disable spring-loading as a drag moves within the bounds of the spring-loading destination or `draggingInfo` changes during the drag.

func springLoadingExited(any NSDraggingInfo)

Responds when a drag exits the bounds of the spring-loading destination.

func draggingEnded(any NSDraggingInfo)

Responds to the end of a drag operation.

