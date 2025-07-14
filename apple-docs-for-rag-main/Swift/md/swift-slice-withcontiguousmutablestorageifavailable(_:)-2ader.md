

- Swift
- Slice
-  withContiguousMutableStorageIfAvailable(\_:) 

Instance Method

# withContiguousMutableStorageIfAvailable(\_:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withContiguousMutableStorageIfAvailable(_ body: (inout UnsafeMutableBufferPointer) throws -> R) rethrows -> R? where Base == UnsafeMutableBufferPointer
```

Available when `Base` conforms to `Collection`.

