

- Paravirtualized Graphics
- PGDisplayDescriptor
-  newFrameEventHandler 

Instance Property

# newFrameEventHandler

A handler that the framework calls when the guest environment has a new frame to display.

Mac Catalyst 14.0+macOS 11.0+

``` source
var newFrameEventHandler: PGDisplayNewFrameEventHandler? { get set }
```

## See Also

### Handling Frame Events

typealias PGDisplayNewFrameEventHandler

The block signature for a routine that handles frame updates from the guest.

