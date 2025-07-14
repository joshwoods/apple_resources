

- ARKit
- ARFrame
- ARFrame.WorldMappingStatus
-  ARFrame.WorldMappingStatus.notAvailable 

Case

# ARFrame.WorldMappingStatus.notAvailable

No world map is available.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case notAvailable
```

## Discussion

When the worldMappingStatus of the session’s currentFrame is ARFrame.WorldMappingStatus.notAvailable, the session has no internal map of the real-world space around the device, nor the scene visible to the camera. Calling getCurrentWorldMap(completionHandler:) at this time results in an error.

This status occurs shortly after starting a new session. To save or share a world map, wait for the user to explore their surroundings and the session’s status to change to ARFrame.WorldMappingStatus.mapped or ARFrame.WorldMappingStatus.extending.

