

- Accelerate
- AccelerateMutableBuffer
-  withUnsafePixelBuffer(body:) 

Instance Method

# withUnsafePixelBuffer(body:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
mutating func withUnsafePixelBuffer(body: (vImage.PixelBuffer) throws -> R) rethrows -> R
```

Available when `Element` is `Float16`.

