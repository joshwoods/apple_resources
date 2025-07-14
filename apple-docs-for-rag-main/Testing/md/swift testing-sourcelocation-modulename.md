

- Swift Testing
- SourceLocation
-  moduleName 

Instance Property

# moduleName

The name of the module containing the source file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var moduleName: String { get }
```

## Discussion

The name of the module is derived from this instance’s fileID property. It consists of the substring of the file ID up to the first forward-slash character (`"/"`.) For example, if the value of this instance’s fileID property is `"FoodTruck/WheelTests.swift"`, the module name is `"FoodTruck"`.

The structure of file IDs is described in the documentation for the #fileID macro in the Swift standard library.

## See Also

### Related Documentation

var fileID: String

The file ID of the source file.

var fileName: String

The name of the source file.

#fileID

