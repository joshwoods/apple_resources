

- Core ML
- MLShapedArray
-  withPixelBufferIfAvailable(\_:) 

Instance Method

# withPixelBufferIfAvailable(\_:)

Reads the underlying pixel buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func withPixelBufferIfAvailable(_ body: (CVPixelBuffer) throws -> R) rethrows -> R?
```

## Parameters 

`body`  

The closure to run with the pixel buffer.

## Return Value

The value returned from body, unless the shaped array doesn’t use a pixel buffer backing, in which case the method ignores body and returns nil.

## Discussion

Use this method to read the contents of the underlying pixel buffer. The pixel buffer is read only. Do not write to it.

```
let array = MLShapedArray(mutating: pixelBuffer, shape: [2, 3])
array.withPixelBuffer { backingPixelBuffer in
     // read backingPixelBuffer here.
}
```

