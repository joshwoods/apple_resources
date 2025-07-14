

- Core Services
- OS Services
- Identity Services
-  CSIdentityClientContext 

Structure

# CSIdentityClientContext

Mac Catalyst 13.0+macOS 10.5+

``` source
struct CSIdentityClientContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: CFAllocatorRetainCallBack!, release: CFAllocatorReleaseCallBack!, copyDescription: CFAllocatorCopyDescriptionCallBack!, statusUpdated: CSIdentityStatusUpdatedCallback!)

### Instance Properties

var copyDescription: CFAllocatorCopyDescriptionCallBack!

var info: UnsafeMutableRawPointer!

var release: CFAllocatorReleaseCallBack!

var retain: CFAllocatorRetainCallBack!

var statusUpdated: CSIdentityStatusUpdatedCallback!

var version: CFIndex

