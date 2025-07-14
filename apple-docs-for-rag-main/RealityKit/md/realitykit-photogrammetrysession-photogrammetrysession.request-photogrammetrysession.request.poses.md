

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
-  PhotogrammetrySession.Request.poses 

Case

# PhotogrammetrySession.Request.poses

Requests the estimated pose of the camera in each shot (relative to the common estimated coordinate system shared with the `.bounds` request).

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
case poses
```

## Discussion

Once initial photogrammetric calculations are complete, a PhotogrammetrySession.Poses object will be returned with the estimated camera pose for each sample that was used in the reconstruction.

