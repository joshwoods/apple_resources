

- AppKit
- NSSpringLoadingOptions
-  noHover 

Type Property

# noHover

Spring-loading on the destination object is enabled, but cannot be invoked by hovering. The user can drag an object over a destination object and force click to initiate spring-loading and activate the destination object. This option may be useful in situations where a long hover, such as dragging across a large destination object, initiates undesired spring-loading. Use this constant sparingly.

macOS 10.11+

``` source
static var noHover: NSSpringLoadingOptions { get }
```

## See Also

### Constants

static var disabled: NSSpringLoadingOptions

Spring-loading on the destination object is disabled. No spring-loading operations can occur.

static var enabled: NSSpringLoadingOptions

Spring-loading on the destination object is enabled. The user can drag an object over a destination object and hover or force click to initiate spring-loading and activate the destination object. When initiated by a force click, spring-loading is invoked once the force click is released.

static var continuousActivation: NSSpringLoadingOptions

Spring-loading on the destination object is enabled. The user can drag an object over a destination object and hover or force click to initiate spring-loading and activate the destination object. When initiated by a force click, spring-loading is invoked once the force click begins and deactivated when the force click is released. When initiated by hovering, spring-loading is invoked at the hover timeout and deactivated when the drag exits the destination object. Use this constant sparingly.

