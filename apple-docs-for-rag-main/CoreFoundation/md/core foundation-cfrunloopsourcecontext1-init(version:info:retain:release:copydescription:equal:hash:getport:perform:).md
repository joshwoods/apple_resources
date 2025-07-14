

- Core Foundation
- CFRunLoopSourceContext1
-  init(version:info:retain:release:copyDescription:equal:hash:getPort:perform:) 

Initializer

# init(version:info:retain:release:copyDescription:equal:hash:getPort:perform:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    version: CFIndex,
    info: UnsafeMutableRawPointer!,
    retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!,
    release: ((UnsafeRawPointer?) -> Void)!,
    copyDescription: ((UnsafeRawPointer?) -> Unmanaged?)!,
    equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!,
    hash: ((UnsafeRawPointer?) -> CFHashCode)!,
    getPort: ((UnsafeMutableRawPointer?) -> mach_port_t)!,
    perform: ((UnsafeMutableRawPointer?, CFIndex, CFAllocator?, UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!
)
```

