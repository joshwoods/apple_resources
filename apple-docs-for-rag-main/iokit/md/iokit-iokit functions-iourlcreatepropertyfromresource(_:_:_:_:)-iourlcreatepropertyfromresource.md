

- IOKit
- IOKit Functions
-  IOURLCreatePropertyFromResource(\_:\_:\_:\_:) 

Function

# IOURLCreatePropertyFromResource(\_:\_:\_:\_:)

Mac Catalyst 13.0+macOS 10.9+Xcode 6.1+

``` source
func IOURLCreatePropertyFromResource(
    _ alloc: CFAllocator!,
    _ url: CFURL!,
    _ property: CFString!,
    _ errorCode: UnsafeMutablePointer!
) -> Unmanaged!
```

