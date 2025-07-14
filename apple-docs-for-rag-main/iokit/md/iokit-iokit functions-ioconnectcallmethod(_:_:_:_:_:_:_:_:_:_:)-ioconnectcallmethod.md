

- IOKit
- IOKit Functions
-  IOConnectCallMethod(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# IOConnectCallMethod(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.5+visionOS 1.0+

``` source
func IOConnectCallMethod(
    _ connection: mach_port_t,
    _ selector: UInt32,
    _ input: UnsafePointer!,
    _ inputCnt: UInt32,
    _ inputStruct: UnsafeRawPointer!,
    _ inputStructCnt: Int,
    _ output: UnsafeMutablePointer!,
    _ outputCnt: UnsafeMutablePointer!,
    _ outputStruct: UnsafeMutableRawPointer!,
    _ outputStructCnt: UnsafeMutablePointer!
) -> kern_return_t
```

