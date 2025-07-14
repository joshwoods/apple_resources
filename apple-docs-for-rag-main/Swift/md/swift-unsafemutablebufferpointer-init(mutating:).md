

- Swift
- UnsafeMutableBufferPointer
-  init(mutating:) 

Initializer

# init(mutating:)

Creates a mutable typed buffer pointer referencing the same memory as the given immutable buffer pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(mutating other: UnsafeBufferPointer)
```

## Parameters 

`other`  

The immutable buffer pointer to convert.

