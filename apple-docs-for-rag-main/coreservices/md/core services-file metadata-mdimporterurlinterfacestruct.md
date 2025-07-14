

- Core Services
- File Metadata
-  MDImporterURLInterfaceStruct 

Structure

# MDImporterURLInterfaceStruct

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
struct MDImporterURLInterfaceStruct
```

## Topics

### Initializers

init()

init(_reserved: UnsafeMutableRawPointer!, QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!, AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!, Release: ((UnsafeMutableRawPointer?) -> ULONG)!, ImporterImportURLData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFURL?) -> DarwinBoolean)!)

### Instance Properties

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var ImporterImportURLData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFURL?) -> DarwinBoolean)!

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var Release: ((UnsafeMutableRawPointer?) -> ULONG)!

