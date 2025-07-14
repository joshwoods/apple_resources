

- Core Services
- OS Services
- Identity Services
-  CSIdentityQueryClientContext 

Structure

# CSIdentityQueryClientContext

Mac Catalyst 13.0+macOS 10.5+

``` source
struct CSIdentityQueryClientContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retainInfo: CFAllocatorRetainCallBack!, releaseInfo: CFAllocatorReleaseCallBack!, copyInfoDescription: CFAllocatorCopyDescriptionCallBack!, receiveEvent: CSIdentityQueryReceiveEventCallback!)

### Instance Properties

var copyInfoDescription: CFAllocatorCopyDescriptionCallBack!

var info: UnsafeMutableRawPointer!

var receiveEvent: CSIdentityQueryReceiveEventCallback!

var releaseInfo: CFAllocatorReleaseCallBack!

var retainInfo: CFAllocatorRetainCallBack!

var version: CFIndex

