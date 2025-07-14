

- IOKit
- IOKit Functions
-  IOURLCreateDataAndPropertiesFromResource(\_:\_:\_:\_:\_:\_:) 

Function

# IOURLCreateDataAndPropertiesFromResource(\_:\_:\_:\_:\_:\_:)

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
func IOURLCreateDataAndPropertiesFromResource(
    _ alloc: CFAllocator!,
    _ url: CFURL!,
    _ resourceData: UnsafeMutablePointer?>!,
    _ properties: UnsafeMutablePointer?>!,
    _ desiredProperties: CFArray!,
    _ errorCode: UnsafeMutablePointer!
) -> Bool
```

