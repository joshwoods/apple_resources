

- IOKit
- IOKit Functions
-  IOURLWriteDataAndPropertiesToResource(\_:\_:\_:\_:) 

Function

# IOURLWriteDataAndPropertiesToResource(\_:\_:\_:\_:)

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
func IOURLWriteDataAndPropertiesToResource(
    _ url: CFURL!,
    _ dataToWrite: CFData!,
    _ propertiesToWrite: CFDictionary!,
    _ errorCode: UnsafeMutablePointer!
) -> Bool
```

