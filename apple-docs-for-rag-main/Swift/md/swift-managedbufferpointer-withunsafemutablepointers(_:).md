

- Swift
- ManagedBufferPointer
-  withUnsafeMutablePointers(\_:) 

Instance Method

# withUnsafeMutablePointers(\_:)

Call `body` with `UnsafeMutablePointer`s to the stored `Header` and raw `Element` storage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withUnsafeMutablePointers(_ body: (UnsafeMutablePointer, UnsafeMutablePointer) throws(E) -> R) throws(E) -> R where E : Error, R : ~Copyable
```

## Discussion

Note

These pointers are valid only for the duration of the call to `body`.

## See Also

### Accessing Buffer Contents

func withUnsafeMutablePointerToElements&lt;E, R>((UnsafeMutablePointer&lt;Element>) throws(E) -> R) throws(E) -> R

Call `body` with an `UnsafeMutablePointer` to the `Element` storage.

func withUnsafeMutablePointerToHeader&lt;E, R>((UnsafeMutablePointer&lt;Header>) throws(E) -> R) throws(E) -> R

Call `body` with an `UnsafeMutablePointer` to the stored `Header`.

