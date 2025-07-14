

- Foundation
- NSString
-  init(bytesNoCopy:length:encoding:deallocator:) 

Initializer

# init(bytesNoCopy:length:encoding:deallocator:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    length len: Int,
    encoding: UInt,
    deallocator: ((UnsafeMutableRawPointer, Int) -> Void)? = nil
)
```

