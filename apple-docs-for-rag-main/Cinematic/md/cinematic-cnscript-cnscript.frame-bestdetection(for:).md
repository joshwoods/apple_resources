

- Cinematic
- CNScript
- CNScript.Frame
-  bestDetection(for:) 

Instance Method

# bestDetection(for:)

The best detection to focus on in a frame among those within the given detection group.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func bestDetection(for detectionGroupID: CNDetectionGroupID) -> CNDetection?
```

## Parameters 

`detectionGroupID`  

Associates related detections.

## Return Value

An object representing the best detection to focus on in a frame among those within the given detection group.

## Discussion

Some types of detections also include a detection group ID that associates related detections, such as a face and torso, of the same person.

