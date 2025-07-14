

- Core Foundation
- CFAllocatorContext
-  init(version:info:retain:release:copyDescription:allocate:reallocate:deallocate:preferredSize:) 

Initializer

# init(version:info:retain:release:copyDescription:allocate:reallocate:deallocate:preferredSize:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    version: CFIndex,
    info: UnsafeMutableRawPointer!,
    retain: CFAllocatorRetainCallBack!,
    release: CFAllocatorReleaseCallBack!,
    copyDescription: CFAllocatorCopyDescriptionCallBack!,
    allocate: CFAllocatorAllocateCallBack!,
    reallocate: CFAllocatorReallocateCallBack!,
    deallocate: CFAllocatorDeallocateCallBack!,
    preferredSize: CFAllocatorPreferredSizeCallBack!
)
```

