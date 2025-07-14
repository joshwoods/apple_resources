

- IOKit
- IOKit Structures
- IOCFPlugInInterfaceStruct
-  init(\_reserved:QueryInterface:AddRef:Release:version:revision:Probe:Start:Stop:) 

Initializer

# init(\_reserved:QueryInterface:AddRef:Release:version:revision:Probe:Start:Stop:)

Mac Catalyst 13.0+macOS 10.9+Xcode 9.0+

``` source
init(
    _reserved: UnsafeMutableRawPointer!,
    QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer?) -> HRESULT)!,
    AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!,
    Release: ((UnsafeMutableRawPointer?) -> ULONG)!,
    version: UInt16,
    revision: UInt16,
    Probe: ((UnsafeMutableRawPointer?, CFDictionary?, io_service_t, UnsafeMutablePointer?) -> IOReturn)!,
    Start: ((UnsafeMutableRawPointer?, CFDictionary?, io_service_t) -> IOReturn)!,
    Stop: ((UnsafeMutableRawPointer?) -> IOReturn)!
)
```

