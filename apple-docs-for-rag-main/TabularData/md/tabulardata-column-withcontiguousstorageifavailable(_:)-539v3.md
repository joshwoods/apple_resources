

- TabularData
- Column
-  withContiguousStorageIfAvailable(\_:) 

Instance Method

# withContiguousStorageIfAvailable(\_:)

This method always returns `nil` without calling `body`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func withContiguousStorageIfAvailable(_ body: (UnsafeBufferPointer) throws -> R) rethrows -> R?
```

## Discussion

Use the version of this method that uses a buffer of non-optional elements.

