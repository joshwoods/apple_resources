

- Swift
- UnsafeBufferPointer
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(i: Int) -> Element { get }
```

## Parameters 

`i`  

The position of the element to access. `i` must be in the range `0..

## Overview

The following example uses the buffer pointer’s subscript to access every other element of the buffer:

```
let numbers = [1, 2, 3, 4, 5]
let sum = numbers.withUnsafeBufferPointer { buffer -> Int in
    var result = 0
    for i in stride(from: buffer.startIndex, to: buffer.endIndex, by: 2) {
        result += buffer[i]
    }
    return result
}
// 'sum' == 9
```

Note

Bounds checks for `i` are performed only in debug mode.

