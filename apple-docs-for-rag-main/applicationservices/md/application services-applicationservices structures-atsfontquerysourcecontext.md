

- Application Services
- ApplicationServices Structures
-  ATSFontQuerySourceContext 

Structure

# ATSFontQuerySourceContext

Mac Catalyst 13.0+macOS 10.2+

``` source
struct ATSFontQuerySourceContext
```

## Topics

### Initializers

init()

init(version: UInt32, refCon: UnsafeMutableRawPointer!, retain: CFAllocatorRetainCallBack!, release: CFAllocatorReleaseCallBack!)

### Instance Properties

var refCon: UnsafeMutableRawPointer!

var release: CFAllocatorReleaseCallBack!

var retain: CFAllocatorRetainCallBack!

var version: UInt32

