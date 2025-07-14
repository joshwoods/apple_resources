

- Swift
- UnsafeMutableRawPointer
-  alignedDown(toMultipleOf:) 

Instance Method

# alignedDown(toMultipleOf:)

Obtain the preceding pointer whose bit pattern is a multiple of `alignment`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func alignedDown(toMultipleOf alignment: Int) -> UnsafeMutableRawPointer
```

## Parameters 

`alignment`  

The alignment of the returned pointer, in bytes. `alignment` must be a whole power of 2.

## Return Value

A pointer aligned to `alignment`.

## Discussion

If the bit pattern of `self` is a multiple of `alignment`, this function returns `self`.

