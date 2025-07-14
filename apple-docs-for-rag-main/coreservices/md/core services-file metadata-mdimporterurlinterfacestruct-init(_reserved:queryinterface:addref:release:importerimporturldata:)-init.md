

- Core Services
- File Metadata
- MDImporterURLInterfaceStruct
-  init(\_reserved:QueryInterface:AddRef:Release:ImporterImportURLData:) 

Initializer

# init(\_reserved:QueryInterface:AddRef:Release:ImporterImportURLData:)

Mac Catalyst 13.0+macOS 10.9+Xcode 9.0+

``` source
init(
    _reserved: UnsafeMutableRawPointer!,
    QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer?) -> HRESULT)!,
    AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!,
    Release: ((UnsafeMutableRawPointer?) -> ULONG)!,
    ImporterImportURLData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFURL?) -> DarwinBoolean)!
)
```

