

- Swift
- ManagedBufferPointer
-  withUnsafeMutablePointerToElements(\_:) 

Instance Method

# withUnsafeMutablePointerToElements(\_:)

Call `body` with an `UnsafeMutablePointer` to the `Element` storage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withUnsafeMutablePointerToElements(_ body: (UnsafeMutablePointer) throws(E) -> R) throws(E) -> R where E : Error, R : ~Copyable
```

## Discussion

Note

This pointer is valid only for the duration of the call to `body`.

## See Also

### Accessing Buffer Contents

func withUnsafeMutablePointerToHeader&lt;E, R>((UnsafeMutablePointer&lt;Header>) throws(E) -> R) throws(E) -> R

Call `body` with an `UnsafeMutablePointer` to the stored `Header`.

func withUnsafeMutablePointers&lt;E, R>((UnsafeMutablePointer&lt;Header>, UnsafeMutablePointer&lt;Element>) throws(E) -> R) throws(E) -> R

Call `body` with `UnsafeMutablePointer`s to the stored `Header` and raw `Element` storage.

