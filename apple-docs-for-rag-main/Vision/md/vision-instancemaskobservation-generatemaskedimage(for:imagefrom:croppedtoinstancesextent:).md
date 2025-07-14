

- Vision
- InstanceMaskObservation
-  generateMaskedImage(for:imageFrom:croppedToInstancesExtent:) 

Instance Method

# generateMaskedImage(for:imageFrom:croppedToInstancesExtent:)

Creates a high-resolution image with everything except for the instances you specify masked out.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func generateMaskedImage(
    for instances: IndexSet,
    imageFrom requestHandler: ImageRequestHandler,
    croppedToInstancesExtent: Bool = false
) throws -> CVPixelBuffer
```

## Parameters 

`instances`  

An indexed set of selected instances, where `0` is the background.

`requestHandler`  

A request handler containing an image to be masked.

`croppedToInstancesExtent`  

Crops the image to the smallest rectangle containing all instances. Default is `false`.

## Return Value

The pixel buffer that contains the image.

## Discussion

## See Also

### Generating a mask

func generateMask(for: IndexSet) throws -> CVPixelBuffer

Creates a low-resolution mask from the instances you specify.

func generateScaledMask(for: IndexSet, scaledToImageFrom: ImageRequestHandler) throws -> CVPixelBuffer

Creates a high-resolution mask representing a combination of the instances you specify.

