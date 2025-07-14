

- Core Image
- CIImageProcessorKernel
-  outputIsOpaque 

Type Property

# outputIsOpaque

Boolean determining whether or not processor outputs an opaque image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class var outputIsOpaque: Bool { get }
```

## Discussion

Override this property if your processor's output stores `1.0` into the alpha channel of all pixels within the output extent. If not overridden, `false` is returned.

