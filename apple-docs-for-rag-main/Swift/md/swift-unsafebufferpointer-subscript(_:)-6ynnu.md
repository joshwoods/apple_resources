

- Swift
- UnsafeBufferPointer
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous subrange of the buffer’s elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(bounds: Range) -> Slice> { get }
```

## Parameters 

`bounds`  

A range of the buffer’s indices. The bounds of the range must be valid indices of the buffer.

## Overview

The accessed slice uses the same indices for the same elements as the original buffer uses. Always use the slice’s `startIndex` property instead of assuming that its indices start at a particular value.

This example demonstrates getting a slice from a buffer of strings, finding the index of one of the strings in the slice, and then using that index in the original buffer.

```
let streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
streets.withUnsafeBufferPointer { buffer in
    let streetSlice = buffer[2..

Note

Bounds checks for `bounds` are performed only in debug mode.

