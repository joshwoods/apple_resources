

- Swift Testing
- SourceLocation
-  fileName 

Instance Property

# fileName

The name of the source file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var fileName: String { get }
```

## Discussion

The name of the source file is derived from this instance’s fileID property. It consists of the substring of the file ID after the last forward-slash character (`"/"`.) For example, if the value of this instance’s fileID property is `"FoodTruck/WheelTests.swift"`, the file name is `"WheelTests.swift"`.

The structure of file IDs is described in the documentation for #fileID in the Swift standard library.

## See Also

### Related Documentation

var fileID: String

The file ID of the source file.

var moduleName: String

The name of the module containing the source file.

