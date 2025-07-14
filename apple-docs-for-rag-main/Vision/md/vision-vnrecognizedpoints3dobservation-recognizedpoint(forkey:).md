

- Vision
- VNRecognizedPoints3DObservation
-  recognizedPoint(forKey:) 

Instance Method

# recognizedPoint(forKey:)

Returns a point for a key you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func recognizedPoint(forKey pointKey: VNRecognizedPointKey) throws -> VNRecognizedPoint3D
```

## Parameters 

`pointKey`  

The key of the point to retrieve.

## Return Value

The point the observation associates with the key.

## See Also

### Inspecting the Observation

var availableKeys: [VNRecognizedPointKey]

The available point keys in the observation.

var availableGroupKeys: [VNRecognizedPointGroupKey]

The available point group keys in the observation.

func recognizedPoints(forGroupKey: VNRecognizedPointGroupKey) throws -> [VNRecognizedPointKey : VNRecognizedPoint3D]

Returns a point for a group key you specify.

