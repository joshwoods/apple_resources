

- Swift
- OpaquePointer
-  init(\_:) 

Initializer

# init(\_:)

Converts a typed `UnsafeMutablePointer` to an opaque C pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(_ from: UnsafeMutablePointer?) where T : ~Copyable
```

## Discussion

The result is `nil` if `from` is `nil`.

