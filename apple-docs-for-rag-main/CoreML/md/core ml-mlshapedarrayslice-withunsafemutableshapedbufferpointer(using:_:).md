

- Core ML
- MLShapedArraySlice
-  withUnsafeMutableShapedBufferPointer(using:\_:) 

Instance Method

# withUnsafeMutableShapedBufferPointer(using:\_:)

Calls the given closure with a pointer to the array’s mutable storage that has a specified buffer layout.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func withUnsafeMutableShapedBufferPointer(
    using bufferLayout: MLShapedArrayBufferLayout,
    _ body: (inout UnsafeMutableBufferPointer, [Int], [Int]) throws -> R
) rethrows -> R
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Discussion

The storage contains the scalars according to buffer layout parameter. For example, the scalar at `[x1, x2, ... xn]` with strides `[s1, s2, ... sn]` is stored at `ptr[x1 * s1 + x2 * s2 + ... + xn * sn]`

Unlike `withUnsafeMutableShapedBufferPointer(:)`, this function allows the caller to specify the buffer layout.

```
// Initialize the middle 2x2 of 4x4 shaped array using an external data that lays out
// scalars in last-major order.
let data: [Int32] = [1, 3,
                     2, 4]
var array = MLShapedArray(repeating: 0, shape: [4, 4])
array[1...2, 1...2].withUnsafeMutableShapedBufferPointer(using: .lastMajorContiguous) { destinationPtr, _, _ in
    data.withUnsafeBufferPointer() { sourcePtr in
        destinationPtr.update(from: sourcePtr)
    }
}

// array.scalars == [0, 0, 0, 0,
//                   0, 1, 2, 0,
//                   0, 3, 4, 0,
//                   0, 0, 0, 0,])
```

