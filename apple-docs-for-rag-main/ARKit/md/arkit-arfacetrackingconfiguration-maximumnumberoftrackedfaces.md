

- ARKit
- ARFaceTrackingConfiguration
-  maximumNumberOfTrackedFaces 

Instance Property

# maximumNumberOfTrackedFaces

The number of faces to track during the session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var maximumNumberOfTrackedFaces: Int { get set }
```

## Discussion

The default value is one. Set the maximum number of tracked faces to limit the number of faces that can be tracked in a given frame. Check the value of supportedNumberOfTrackedFaces before setting this property.

No new anchors will be provided to your delegate’s session(_:didAdd:) if more than the maximum number of faces are visible in the camera feed. In that case, ARKit continues to track the faces that already have associated face anchors.

## See Also

### Tracking Multiple Faces

class var supportedNumberOfTrackedFaces: Int

The maximum number of faces that the framework can track.

