

- Vision
- VNRecognizedPointsObservation
-  recognizedPoints(forGroupKey:) 

Instance Method

# recognizedPoints(forGroupKey:)

Retrieves the recognized points for a key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func recognizedPoints(forGroupKey groupKey: VNRecognizedPointGroupKey) throws -> [VNRecognizedPointKey : VNRecognizedPoint]
```

## Parameters 

`groupKey`  

The group key to retrieve recognized points for.

## Return Value

A dictionary of labeled points for the group.

## See Also

### Inspecting the Observation

var availableKeys: [VNRecognizedPointKey]

The available point keys in the observation.

var availableGroupKeys: [VNRecognizedPointGroupKey]

The available point group keys in the observation.

func recognizedPoint(forKey: VNRecognizedPointKey) throws -> VNRecognizedPoint

Retrieves a recognized point for a key.

