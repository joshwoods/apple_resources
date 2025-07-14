

- Accelerate
- vImage
- vImage.CompositeMode
-  vImage.CompositeMode.premultipliedWithConstantAlpha(\_:) 

Case

# vImage.CompositeMode.premultipliedWithConstantAlpha(\_:)

Performs premultiplied alpha compositing of two images, using a single alpha value for the entire image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
case premultipliedWithConstantAlpha(ComponentType)
```

## See Also

### Enumeration Cases

case nonpremultiplied

Composite two non-premultiplied images, to produce a non-premultiplied result.

case nonpremultipliedToPremultiplied

Blends a nonpremultiplied top image into a premultiplied bottom image and returns a premultiplied result.

case premultiplied

Blends two premultiplied images to produce a premultiplied result.

