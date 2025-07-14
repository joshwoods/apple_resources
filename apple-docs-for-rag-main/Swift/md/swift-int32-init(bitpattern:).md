

- Swift
- Int32
-  init(bitPattern:) 

Initializer

# init(bitPattern:)

Creates a new instance with the same memory representation as the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(bitPattern x: UInt32)
```

## Parameters 

`x`  

A value to use as the source of the new instance’s binary representation.

## Discussion

This initializer does not perform any range or overflow checking. The resulting instance may not have the same numeric value as `bitPattern`—it is only guaranteed to use the same pattern of bits in its binary representation.

