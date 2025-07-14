

- Core Foundation
- CFRunLoopSourceContext
-  init(version:info:retain:release:copyDescription:equal:hash:schedule:cancel:perform:) 

Initializer

# init(version:info:retain:release:copyDescription:equal:hash:schedule:cancel:perform:)

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
    schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!,
    cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!,
    perform: ((UnsafeMutableRawPointer?) -> Void)!
)
```

