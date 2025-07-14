

- Core Image
- CIImageProcessorKernel
-  synchronizeInputs 

Type Property

# synchronizeInputs

Tells whether or not processor input should be synchronized for CPU access.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class var synchronizeInputs: Bool { get }
```

## Discussion

Set to return `false` if you want your processor to be given CIImageProcessorInput objects not synchronized for CPU access.Set to return `false` if your subclass uses the GPU.

Defaults to `true` if not overridden.

