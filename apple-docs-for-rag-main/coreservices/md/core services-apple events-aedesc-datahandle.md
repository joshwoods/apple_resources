

- Core Services
- Apple Events
- AEDesc
-  dataHandle 

Instance Property

# dataHandle

An opaque storage type that points to the storagefor the descriptor data. Your application doesn’t access thisdata directly—rather, it calls one of the functions AEGetDescDataSize(_:), AEGetDescData(_:_:_:), or AEReplaceDescData(_:_:_:_:).See AEDataStorage.

Mac Catalyst 13.0+macOS 10.0+

``` source
var dataHandle: AEDataStorage!
```

