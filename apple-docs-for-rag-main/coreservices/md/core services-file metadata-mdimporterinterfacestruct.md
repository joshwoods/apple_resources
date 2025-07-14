

- Core Services
- File Metadata
-  MDImporterInterfaceStruct 

Structure

# MDImporterInterfaceStruct

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
struct MDImporterInterfaceStruct
```

## Topics

### Initializers

init()

init(_reserved: UnsafeMutableRawPointer!, QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!, AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!, Release: ((UnsafeMutableRawPointer?) -> ULONG)!, ImporterImportData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFString?) -> DarwinBoolean)!)

### Instance Properties

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var ImporterImportData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFString?) -> DarwinBoolean)!

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var Release: ((UnsafeMutableRawPointer?) -> ULONG)!

