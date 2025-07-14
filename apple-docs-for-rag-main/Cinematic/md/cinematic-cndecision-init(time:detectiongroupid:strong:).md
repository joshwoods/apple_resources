

- Cinematic
- CNDecision
-  init(time:detectionGroupID:strong:) 

Initializer

# init(time:detectionGroupID:strong:)

Makes a decision to focus on the detection with the given unique detection.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
init(
    time: CMTime,
    detectionGroupID: CNDetectionGroupID,
    strong isStrong: Bool
)
```

## Parameters 

`time`  

The first presentation time which the subject should be in focus.

`detectionGroupID`  

The unique detection representing the detection to focus on if this isn’t a group decision.

`isStrong`  

A flag representing whether this is a strong decision or not. A strong decision keeps focus for as long as possible.

## Discussion

A strong decision keeps focus for as long as possible on the detected subject.

## See Also

### Initializers

init(time: CMTime, detectionID: CNDetectionID, strong: Bool)

Makes a decision to focus on the best among those detections with the same detection group ID.

