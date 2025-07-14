

- Vision
- VNInstanceMaskObservation
-  generateScaledMaskForImage(forInstances:from:) 

Instance Method

# generateScaledMaskForImage(forInstances:from:)

Creates a high-resolution mask where everything becomes transparent black, except for the instances you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func generateScaledMaskForImage(
    forInstances instances: IndexSet,
    from requestHandler: VNImageRequestHandler
) throws -> CVPixelBuffer
```

## Parameters 

`instances`  

The collection of instances.

`requestHandler`  

The image request callback.

## Return Value

The pixel buffer that contains the image.

## See Also

### Creating a Mask

func generateMask(forInstances: IndexSet) throws -> CVPixelBuffer

Creates a low-resolution mask from the instances you specify.

func generateMaskedImage(ofInstances: IndexSet, from: VNImageRequestHandler, croppedToInstancesExtent: Bool) throws -> CVPixelBuffer

Creates a high-resolution image where everything becomes transparent black, except for the instances you specify.

