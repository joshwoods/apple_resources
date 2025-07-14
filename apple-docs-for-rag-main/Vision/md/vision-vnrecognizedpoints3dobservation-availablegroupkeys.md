

- Vision
- VNRecognizedPoints3DObservation
-  availableGroupKeys 

Instance Property

# availableGroupKeys

The available point group keys in the observation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var availableGroupKeys: [VNRecognizedPointGroupKey] { get }
```

## See Also

### Inspecting the Observation

var availableKeys: [VNRecognizedPointKey]

The available point keys in the observation.

func recognizedPoint(forKey: VNRecognizedPointKey) throws -> VNRecognizedPoint3D

Returns a point for a key you specify.

func recognizedPoints(forGroupKey: VNRecognizedPointGroupKey) throws -> [VNRecognizedPointKey : VNRecognizedPoint3D]

Returns a point for a group key you specify.

