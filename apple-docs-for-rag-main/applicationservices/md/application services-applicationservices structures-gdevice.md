

- Application Services
- ApplicationServices Structures
-  GDevice 

Structure

# GDevice

macOS 10.0+

``` source
struct GDevice
```

## Topics

### Initializers

init()

init(gdRefNum: Int16, gdID: Int16, gdType: Int16, gdITable: Handle!, gdResPref: Int16, gdSearchProc: Handle!, gdCompProc: Handle!, gdFlags: Int16, gdPMap: PixMapHandle!, gdRefCon: Int32, gdNextGD: GDHandle!, gdRect: Rect, gdMode: Int32, gdCCBytes: Int16, gdCCDepth: Int16, gdCCXData: Handle!, gdCCXMask: Handle!, gdExt: Handle!)

### Instance Properties

var gdCCBytes: Int16

var gdCCDepth: Int16

var gdCCXData: Handle!

var gdCCXMask: Handle!

var gdCompProc: Handle!

var gdExt: Handle!

var gdFlags: Int16

var gdID: Int16

var gdITable: Handle!

var gdMode: Int32

var gdNextGD: GDHandle!

var gdPMap: PixMapHandle!

var gdRect: Rect

var gdRefCon: Int32

var gdRefNum: Int16

var gdResPref: Int16

var gdSearchProc: Handle!

var gdType: Int16

