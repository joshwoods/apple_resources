

- Core Services
- File Metadata
-  MDExporterInterfaceStruct 

Structure

# MDExporterInterfaceStruct

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
struct MDExporterInterfaceStruct
```

## Topics

### Initializers

init()

init(_reserved: UnsafeMutableRawPointer!, QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!, AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!, Release: ((UnsafeMutableRawPointer?) -> ULONG)!, ImporterExportData: ((UnsafeMutableRawPointer?, CFDictionary?, CFString?, CFString?) -> DarwinBoolean)!)

### Instance Properties

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var ImporterExportData: ((UnsafeMutableRawPointer?, CFDictionary?, CFString?, CFString?) -> DarwinBoolean)!

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var Release: ((UnsafeMutableRawPointer?) -> ULONG)!

