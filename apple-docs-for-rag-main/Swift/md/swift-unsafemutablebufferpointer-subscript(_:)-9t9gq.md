

- Swift
- UnsafeMutableBufferPointer
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(i: Int) -> Element { get nonmutating set }
```

## Parameters 

`i`  

The position of the element to access. `i` must be in the range `0..

## Overview

The following example uses the buffer pointer’s subscript to access and modify the elements of a mutable buffer pointing to the contiguous contents of an array:

```
var numbers = [1, 2, 3, 4, 5]
numbers.withUnsafeMutableBufferPointer { buffer in
    for i in stride(from: buffer.startIndex, to: buffer.endIndex - 1, by: 2) {
        let x = buffer[i]
        buffer[i + 1] = buffer[i]
        buffer[i] = x
    }
}
print(numbers)
// Prints "[2, 1, 4, 3, 5]"

Uninitialized memory cannot be initialized to a nontrivial type
using this subscript. Instead, use an initializing method, such as
`initializeElement(at:to:)`
```

Note

Bounds checks for `i` are performed only in debug mode.

