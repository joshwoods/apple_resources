

- Swift
- UInt
-  init(bitPattern:) 

Initializer

# init(bitPattern:)

Creates a new value with the bit pattern of the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(bitPattern pointer: OpaquePointer?)
```

## Parameters 

`pointer`  

The pointer to use as the source for the new integer.

## Discussion

The new value represents the address of the pointer passed as `pointer`. If `pointer` is `nil`, the result is `0`.

