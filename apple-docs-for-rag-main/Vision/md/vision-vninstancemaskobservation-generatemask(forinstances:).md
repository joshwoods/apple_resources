

- Vision
- VNInstanceMaskObservation
-  generateMask(forInstances:) 

Instance Method

# generateMask(forInstances:)

Creates a low-resolution mask from the instances you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func generateMask(forInstances instances: IndexSet) throws -> CVPixelBuffer
```

## Parameters 

`instances`  

The collection of instances.

## Return Value

The pixel buffer that contains the image.

## See Also

### Creating a Mask

func generateMaskedImage(ofInstances: IndexSet, from: VNImageRequestHandler, croppedToInstancesExtent: Bool) throws -> CVPixelBuffer

Creates a high-resolution image where everything becomes transparent black, except for the instances you specify.

func generateScaledMaskForImage(forInstances: IndexSet, from: VNImageRequestHandler) throws -> CVPixelBuffer

Creates a high-resolution mask where everything becomes transparent black, except for the instances you specify.

