

- Paravirtualized Graphics
-  PGDisplayNewFrameEventHandler 

Type Alias

# PGDisplayNewFrameEventHandler

The block signature for a routine that handles frame updates from the guest.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGDisplayNewFrameEventHandler = () -> Void
```

## See Also

### Handling Frame Events

var newFrameEventHandler: PGDisplayNewFrameEventHandler?

A handler that the framework calls when the guest environment has a new frame to display.

