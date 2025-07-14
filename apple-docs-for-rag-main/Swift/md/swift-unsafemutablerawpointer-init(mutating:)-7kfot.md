

- Swift
- UnsafeMutableRawPointer
-  init(mutating:) 

Initializer

# init(mutating:)

Creates a new mutable raw pointer from the given immutable raw pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(mutating other: UnsafeRawPointer)
```

## Parameters 

`other`  

The immutable raw pointer to convert.

## Discussion

Use this initializer to explicitly convert `other` to an `UnsafeMutableRawPointer` instance. This initializer creates a new pointer to the same address as `other` and performs no allocation or copying.

