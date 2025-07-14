

- Core Foundation
- CFBinaryHeapCallBacks
-  init(version:retain:release:copyDescription:compare:) 

Initializer

# init(version:retain:release:copyDescription:compare:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    version: CFIndex,
    retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!,
    release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!,
    copyDescription: ((UnsafeRawPointer?) -> Unmanaged?)!,
    compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!
)
```

