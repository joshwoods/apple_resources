

- Swift
- UnsafeMutablePointer
-  init(mutating:) 

Initializer

# init(mutating:)

Creates a mutable typed pointer referencing the same memory as the given immutable pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(mutating other: UnsafePointer?)
```

## Parameters 

`other`  

The immutable pointer to convert. If `other` is `nil`, the result is `nil`.

