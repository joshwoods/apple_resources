

- Nearby Interaction
- NISession
-  setARSession(\_:) 

Instance Method

# setARSession(\_:)

Provides the framework with an existing AR session to use for Camera Assistance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func setARSession(_ session: ARSession)
```

## Parameters 

`session`  

An existing AR session configured as follows:

- A world-tracking configuration (ARWorldTrackingConfiguration) with worldAlignment `=` ARConfiguration.WorldAlignment.gravity, isCollaborationEnabled `=` `false`, userFaceTrackingEnabled `=` `false`, and initialWorldMap `=` `nil`.

- A delegate that returns `false` for sessionShouldAttemptRelocalization(_:).

## Discussion

Set the isCameraAssistanceEnabled flag to `true` before calling this function. If you enable the flag and run a nearby-interaction session without calling setARSession(_:), the framework creates an internal ARSession instance to which the app has no access.

## See Also

### Utilizing Camera Assistance

func worldTransform(for: NINearbyObject) -> simd_float4x4?

Returns a world transform to integrate a nearby object in an AR experience.

