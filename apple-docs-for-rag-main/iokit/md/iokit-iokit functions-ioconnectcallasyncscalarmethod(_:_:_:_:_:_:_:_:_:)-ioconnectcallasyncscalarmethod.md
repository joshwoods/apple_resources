

- IOKit
- IOKit Functions
-  IOConnectCallAsyncScalarMethod(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# IOConnectCallAsyncScalarMethod(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.5+visionOS 1.0+

``` source
func IOConnectCallAsyncScalarMethod(
    _ connection: mach_port_t,
    _ selector: UInt32,
    _ wake_port: mach_port_t,
    _ reference: UnsafeMutablePointer!,
    _ referenceCnt: UInt32,
    _ input: UnsafePointer!,
    _ inputCnt: UInt32,
    _ output: UnsafeMutablePointer!,
    _ outputCnt: UnsafeMutablePointer!
) -> kern_return_t
```

