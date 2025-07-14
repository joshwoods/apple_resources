

- Swift
- UnsafeRawPointer
-  init(\_:) 

Initializer

# init(\_:)

Creates a new raw pointer from the given mutable raw pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(_ other: UnsafeMutableRawPointer?)
```

## Parameters 

`other`  

The mutable raw pointer to convert. If `other` is `nil`, the result is `nil`.

## Discussion

Use this initializer to explicitly convert `other` to an `UnsafeRawPointer` instance. This initializer creates a new pointer to the same address as `other` and performs no allocation or copying.

