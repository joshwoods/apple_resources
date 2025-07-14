

- Swift
- ManagedBuffer
-  withUnsafeMutablePointerToHeader(\_:) 

Instance Method

# withUnsafeMutablePointerToHeader(\_:)

Call `body` with an `UnsafeMutablePointer` to the stored `Header`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
final func withUnsafeMutablePointerToHeader(_ body: (UnsafeMutablePointer) throws(E) -> R) throws(E) -> R where E : Error, R : ~Copyable
```

## Discussion

Note

This pointer is valid only for the duration of the call to `body`.

