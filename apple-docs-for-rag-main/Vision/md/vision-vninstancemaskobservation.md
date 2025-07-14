

- Vision
-  VNInstanceMaskObservation 

Class

# VNInstanceMaskObservation

An observation that contains an instance mask that labels instances in the mask.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNInstanceMaskObservation
```

## Topics

### Accessing Instances

var allInstances: IndexSet

The collection that contains all instances, excluding the background.

var instanceMask: CVPixelBuffer

The resulting mask that represents all instances.

### Creating a Mask

func generateMask(forInstances: IndexSet) throws -> CVPixelBuffer

Creates a low-resolution mask from the instances you specify.

func generateMaskedImage(ofInstances: IndexSet, from: VNImageRequestHandler, croppedToInstancesExtent: Bool) throws -> CVPixelBuffer

Creates a high-resolution image where everything becomes transparent black, except for the instances you specify.

func generateScaledMaskForImage(forInstances: IndexSet, from: VNImageRequestHandler) throws -> CVPixelBuffer

Creates a high-resolution mask where everything becomes transparent black, except for the instances you specify.

## Relationships

### Inherits From

- VNObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Image background removal

Applying visual effects to foreground subjects

Segment the foreground subjects of an image and composite them to a new background with visual effects.

class VNGenerateForegroundInstanceMaskRequest

A request that generates an instance mask of noticable objects to separate from the background.

let VNGenerateForegroundInstanceMaskRequestRevision1: Int

A constant for specifying the first revision of the foreground instance mask request.

