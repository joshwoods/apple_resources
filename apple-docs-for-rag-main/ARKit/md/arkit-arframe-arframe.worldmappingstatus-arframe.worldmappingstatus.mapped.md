

- ARKit
- ARFrame
- ARFrame.WorldMappingStatus
-  ARFrame.WorldMappingStatus.mapped 

Case

# ARFrame.WorldMappingStatus.mapped

World tracking has adequately mapped the visible area.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case mapped
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

When the worldMappingStatus of the session’s currentFrame is ARFrame.WorldMappingStatus.mapped, the session has produced a high-fidelity internal map of the real-world space around the device’s current position and the scene visible to the camera.

This status provides the highest reliability for relocalizing to a saved world map, provided that:

1.  You call getCurrentWorldMap(completionHandler:) to save the world map while the status of the currentFrame is ARFrame.WorldMappingStatus.mapped.

2.  When you run a new session (later or on another device) from that ARWorldMap, the device running the new session is at a real-world position and orientation similar to that when the world map was saved.

