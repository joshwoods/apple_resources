

- Vision
- InstanceMaskObservation
-  generateScaledMask(for:scaledToImageFrom:) 

Instance Method

# generateScaledMask(for:scaledToImageFrom:)

Creates a high-resolution mask representing a combination of the instances you specify.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func generateScaledMask(
    for instances: IndexSet,
    scaledToImageFrom requestHandler: ImageRequestHandler
) throws -> CVPixelBuffer
```

## Parameters 

`instances`  

An indexed set of selected instances, where `0` is the background.

`requestHandler`  

A request handler containing an image to be masked.

## Return Value

The pixel buffer that contains the mask.

## See Also

### Generating a mask

func generateMask(for: IndexSet) throws -> CVPixelBuffer

Creates a low-resolution mask from the instances you specify.

func generateMaskedImage(for: IndexSet, imageFrom: ImageRequestHandler, croppedToInstancesExtent: Bool) throws -> CVPixelBuffer

Creates a high-resolution image with everything except for the instances you specify masked out.

