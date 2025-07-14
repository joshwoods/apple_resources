

- Dispatch
- DispatchIO
-  init(type:path:oflag:mode:queue:cleanupHandler:) 

Initializer

# init(type:path:oflag:mode:queue:cleanupHandler:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    type: DispatchIO.StreamType,
    path: UnsafePointer,
    oflag: Int32,
    mode: mode_t,
    queue: DispatchQueue,
    cleanupHandler: @escaping (Int32) -> Void
)
```

