

- Core Services
- File Metadata
- MDImporterInterfaceStruct
-  init(\_reserved:QueryInterface:AddRef:Release:ImporterImportData:) 

Initializer

# init(\_reserved:QueryInterface:AddRef:Release:ImporterImportData:)

Mac Catalyst 13.0+macOS 10.9+Xcode 9.0+

``` source
init(
    _reserved: UnsafeMutableRawPointer!,
    QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer?) -> HRESULT)!,
    AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!,
    Release: ((UnsafeMutableRawPointer?) -> ULONG)!,
    ImporterImportData: ((UnsafeMutableRawPointer?, CFMutableDictionary?, CFString?, CFString?) -> DarwinBoolean)!
)
```

