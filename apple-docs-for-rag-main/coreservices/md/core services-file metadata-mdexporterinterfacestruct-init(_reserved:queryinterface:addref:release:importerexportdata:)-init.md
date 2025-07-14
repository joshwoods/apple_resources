

- Core Services
- File Metadata
- MDExporterInterfaceStruct
-  init(\_reserved:QueryInterface:AddRef:Release:ImporterExportData:) 

Initializer

# init(\_reserved:QueryInterface:AddRef:Release:ImporterExportData:)

Mac Catalyst 13.0+macOS 10.9+Xcode 9.0+

``` source
init(
    _reserved: UnsafeMutableRawPointer!,
    QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer?) -> HRESULT)!,
    AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!,
    Release: ((UnsafeMutableRawPointer?) -> ULONG)!,
    ImporterExportData: ((UnsafeMutableRawPointer?, CFDictionary?, CFString?, CFString?) -> DarwinBoolean)!
)
```

