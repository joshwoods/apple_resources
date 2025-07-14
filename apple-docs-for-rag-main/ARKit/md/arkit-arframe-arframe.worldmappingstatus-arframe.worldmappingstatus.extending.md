

- ARKit
- ARFrame
- ARFrame.WorldMappingStatus
-  ARFrame.WorldMappingStatus.extending 

Case

# ARFrame.WorldMappingStatus.extending

World tracking has mapped recently visited areas, but is still mapping around the current device position.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case extending
```

## Discussion

When the worldMappingStatus of the session’s currentFrame is ARFrame.WorldMappingStatus.extending, the session has produced a high-fidelity internal map of the real-world spaces the device has recently passed thorugh, but is still collecting data to map the area around the device’s current position and the scene visible to the camera.

This status provides moderate to high reliability for relocalizing to a saved world map, provided that:

1.  You call getCurrentWorldMap(completionHandler:) to save the world map while the status of the currentFrame is ARFrame.WorldMappingStatus.extending.

2.  When you run a new session (later or on another device) from that ARWorldMap, the device running the new session passes through positions and orientations that were visited by the device that saved the session.

Saving or sharing a world map at this time is likely to produce adequate results, but a higher quality world map may be possible if you wait until the user explores more of their surroundings and the status changes to ARFrame.WorldMappingStatus.mapped.

