

- Application Services
- ApplicationServices Structures
- PixMap
-  init(baseAddr:rowBytes:bounds:pmVersion:packType:packSize:hRes:vRes:pixelType:pixelSize:cmpCount:cmpSize:pixelFormat:pmTable:pmExt:) 

Initializer

# init(baseAddr:rowBytes:bounds:pmVersion:packType:packSize:hRes:vRes:pixelType:pixelSize:cmpCount:cmpSize:pixelFormat:pmTable:pmExt:)

Mac Catalyst 13.0+macOS 10.9+Xcode 9.0+

``` source
init(
    baseAddr: Ptr!,
    rowBytes: Int16,
    bounds: Rect,
    pmVersion: Int16,
    packType: Int16,
    packSize: Int32,
    hRes: Fixed,
    vRes: Fixed,
    pixelType: Int16,
    pixelSize: Int16,
    cmpCount: Int16,
    cmpSize: Int16,
    pixelFormat: OSType,
    pmTable: CTabHandle!,
    pmExt: UnsafeMutableRawPointer!
)
```

