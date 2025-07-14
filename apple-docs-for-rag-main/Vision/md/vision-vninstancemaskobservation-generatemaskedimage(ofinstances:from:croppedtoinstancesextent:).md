

- Vision
- VNInstanceMaskObservation
-  generateMaskedImage(ofInstances:from:croppedToInstancesExtent:) 

Instance Method

# generateMaskedImage(ofInstances:from:croppedToInstancesExtent:)

Creates a high-resolution image where everything becomes transparent black, except for the instances you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func generateMaskedImage(
    ofInstances instances: IndexSet,
    from requestHandler: VNImageRequestHandler,
    croppedToInstancesExtent cropResult: Bool
) throws -> CVPixelBuffer
```

## Parameters 

`instances`  

The collection of instances.

`requestHandler`  

The image request callback.

`cropResult`  

A Boolean value that indicates whether to crop the image to the smallest rectangle that contains all instances.

## Return Value

The pixel buffer that contains the image.

## See Also

### Creating a Mask

func generateMask(forInstances: IndexSet) throws -> CVPixelBuffer

Creates a low-resolution mask from the instances you specify.

func generateScaledMaskForImage(forInstances: IndexSet, from: VNImageRequestHandler) throws -> CVPixelBuffer

Creates a high-resolution mask where everything becomes transparent black, except for the instances you specify.

