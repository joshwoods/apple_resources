

- TabularData
- Column
-  withContiguousMutableStorageIfAvailable(\_:) 

Instance Method

# withContiguousMutableStorageIfAvailable(\_:)

Call `body(buffer)`, where `buffer` provides access to the non-optional contiguous mutable storage of the entire column. If the column contains missing values, `body` is not called and `nil` is returned.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func withContiguousMutableStorageIfAvailable(_ body: (inout UnsafeMutableBufferPointer) throws -> R) rethrows -> R?
```

## Parameters 

`body`  

A closure to be executed using the elements of this collection.

## Return Value

The value returned by `body`, or `nil`.

## Discussion

The optimizer can often eliminate bounds- and uniqueness-checking within an algorithm. When that fails, however, invoking the same algorithm on `body`’s argument may let you trade safety for speed.

Note

`buffer` must not be replaced by `body`.

