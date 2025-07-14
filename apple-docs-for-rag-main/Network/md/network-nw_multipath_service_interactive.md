

- Network
-  nw_multipath_service_interactive 

Global Variable

# nw_multipath_service_interactive

Enable multipath to use other interfaces when the primary interface encounters loss or delay.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
var nw_multipath_service_interactive: nw_multipath_service_t { get }
```

## See Also

### Multipath service types

var nw_multipath_service_disabled: nw_multipath_service_t

Disable multipath.

var nw_multipath_service_handover: nw_multipath_service_t

Enable multipath, but only use other interfaces when the primary interface is lost.

var nw_multipath_service_aggregate: nw_multipath_service_t

Enable multipath to maximize bandwidth across multiple interfaces.

