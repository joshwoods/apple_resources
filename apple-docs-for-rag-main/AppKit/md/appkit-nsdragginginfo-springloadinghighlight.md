

- AppKit
- NSDraggingInfo
-  springLoadingHighlight 

Instance Property

# springLoadingHighlight

A highlighting style for your app’s user interface to display during a spring-loading operation.

macOS 10.11+

``` source
@MainActor
var springLoadingHighlight: NSSpringLoadingHighlight { get }
```

**Required**

## Discussion

During a spring-loaded operation, a destination may initiate animated highlighting to visually cue the user that spring-loading has been engaged or disengaged.

This property contains a highlight style of class NSSpringLoadingHighlight—no highlight, standard highlight, or emphasized highlight. Use this value to update your destination’s user interface accordingly to reflect the appropriate highlight style.

Important

Do not use highlighting as a means to determine whether spring-loading has actually been activated or deactivated. The springLoadingActivated(_:draggingInfo:) method alerts your app when spring-loading activation occurs.

## See Also

### Related Documentation

func springLoadingHighlightChanged(any NSDraggingInfo)

Updates the destination’s user interface to display a new highlighting style during a spring-loading operation.

**Required**

enum NSSpringLoadingHighlight

A group of constants that indicate a highlighting style for your app’s user interface to display during a spring-loading operation.

protocol NSSpringLoadingDestination

A set of methods that the destination object (or recipient) of a dragged object can implement to support spring-loading.

### Implementing spring-loading support

func resetSpringLoading()

Resets a spring-loading operation to its initial state.

**Required**

