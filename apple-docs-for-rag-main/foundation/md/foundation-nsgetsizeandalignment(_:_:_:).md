

- Foundation
-  NSGetSizeAndAlignment(\_:\_:\_:) 

Function

# NSGetSizeAndAlignment(\_:\_:\_:)

Obtains the actual size and the aligned size of an encoded type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSGetSizeAndAlignment(
    _ typePtr: UnsafePointer,
    _ sizep: UnsafeMutablePointer?,
    _ alignp: UnsafeMutablePointer?
) -> UnsafePointer
```

## Discussion

Obtains the actual size and the aligned size of the first data type represented by `typePtr` and returns a pointer to the position of the next data type in `typePtr`. You can specify `NULL` for either `sizep` or `alignp` to ignore the corresponding information.

The value returned in `alignp` is the aligned size of the data type; for example, on some platforms, the aligned size of a `char` might be 2 bytes while the actual physical size is 1 byte.

