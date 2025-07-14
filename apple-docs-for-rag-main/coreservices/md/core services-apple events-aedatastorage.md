

- Core Services
- Apple Events
-  AEDataStorage 

Type Alias

# AEDataStorage

A pointer to an opaque data type that provides storage for an `AEDesc` descriptor.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEDataStorage = UnsafeMutablePointer
```

## Discussion

The Apple Event Manager defines the `AEDataStorage` data type to serve as a data storage field in the AEDesc structure. Your application doesn’t access the data pointed to by a data storage pointer directly. Rather, you work with the following functions:

- AEGetDescDataSize(_:)

- AEGetDescData(_:_:_:)

- AEGetDescDataRange(_:_:_:_:)

- AEReplaceDescData(_:_:_:_:)

