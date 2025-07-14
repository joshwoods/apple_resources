

- Core ML
- MLShapedArray
-  withMutablePixelBufferIfAvailable(\_:) 

Instance Method

# withMutablePixelBufferIfAvailable(\_:)

Writes to the underlying pixel buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func withMutablePixelBufferIfAvailable(_ body: (CVPixelBuffer) throws -> R) rethrows -> R?
```

## Parameters 

`body`  

The closure to run with the pixel buffer.

## Discussion

Use this method to writes the contents of the underlying pixel buffer.

```
let array = MLShapedArray(mutating: pixelBuffer, shape: [2, 3])
array.withMutablePixelBuffer { backingPixelBuffer in
     // write backingPixelBuffer here.
}
```

