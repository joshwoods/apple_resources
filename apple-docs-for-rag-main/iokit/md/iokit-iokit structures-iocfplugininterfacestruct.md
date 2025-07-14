

- IOKit
- IOKit Structures
-  IOCFPlugInInterfaceStruct 

Type Alias

# IOCFPlugInInterfaceStruct

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias IOCFPlugInInterface = IOCFPlugInInterfaceStruct
```

``` source
struct IOCFPlugInInterfaceStruct
```

## Topics

### Initializers

init()

init(_reserved: UnsafeMutableRawPointer!, QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!, AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!, Release: ((UnsafeMutableRawPointer?) -> ULONG)!, version: UInt16, revision: UInt16, Probe: ((UnsafeMutableRawPointer?, CFDictionary?, io_service_t, UnsafeMutablePointer&lt;Int32>?) -> IOReturn)!, Start: ((UnsafeMutableRawPointer?, CFDictionary?, io_service_t) -> IOReturn)!, Stop: ((UnsafeMutableRawPointer?) -> IOReturn)!)

### Instance Properties

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var Probe: ((UnsafeMutableRawPointer?, CFDictionary?, io_service_t, UnsafeMutablePointer&lt;Int32>?) -> IOReturn)!

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var Release: ((UnsafeMutableRawPointer?) -> ULONG)!

var Start: ((UnsafeMutableRawPointer?, CFDictionary?, io_service_t) -> IOReturn)!

var Stop: ((UnsafeMutableRawPointer?) -> IOReturn)!

var revision: UInt16

var version: UInt16

