

- Core Services
- File Metadata
-  MDImporterBundleWrapperURLInterfaceStruct 

Structure

# MDImporterBundleWrapperURLInterfaceStruct

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
struct MDImporterBundleWrapperURLInterfaceStruct
```

## Topics

### Initializers

init()

init(_reserved: UnsafeMutableRawPointer!, QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!, AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!, Release: ((UnsafeMutableRawPointer?) -> ULONG)!, ImporterImportBundleWrapperURLData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFURL?) -> DarwinBoolean)!)

### Instance Properties

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var ImporterImportBundleWrapperURLData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFURL?) -> DarwinBoolean)!

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var Release: ((UnsafeMutableRawPointer?) -> ULONG)!

