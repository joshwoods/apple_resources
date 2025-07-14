

- ARKit
- ARFrame
- ARFrame.WorldMappingStatus
-  ARFrame.WorldMappingStatus.limited 

Case

# ARFrame.WorldMappingStatus.limited

World tracking has not yet sufficiently mapped the area around the current device position.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case limited
```

## Discussion

When the worldMappingStatus of the session’s currentFrame is ARFrame.WorldMappingStatus.limited, the session has not yet fully mapped the real-world space around the device, nor the scene visible to the camera.

Although it is possible at this time to save a world map by calling getCurrentWorldMap(completionHandler:), the resulting ARWorldMap is unlikely to be useful for relocalization in the real-world space near the device’s current position.

To produce a higher quality world map, wait for the user to explore more of their surroundings and the session’s status to change to ARFrame.WorldMappingStatus.mapped or ARFrame.WorldMappingStatus.extending.

