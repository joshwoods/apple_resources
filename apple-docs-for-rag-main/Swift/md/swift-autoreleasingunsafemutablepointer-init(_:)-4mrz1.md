

- Swift
- AutoreleasingUnsafeMutablePointer
-  init(\_:) 

Initializer

# init(\_:)

Explicit construction from an UnsafeMutablePointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ from: UnsafeMutablePointer)
```

## Discussion

This is inherently unsafe; UnsafeMutablePointer assumes the referenced memory has +1 strong ownership semantics, whereas AutoreleasingUnsafeMutablePointer implies +0 semantics.

Warning

Accessing `pointee` as a type that is unrelated to the underlying memory’s bound type is undefined.

## See Also

### Converting Pointers

init?&lt;U>(UnsafeMutablePointer&lt;U>?)

Explicit construction from an UnsafeMutablePointer.

