

- RealityKit
- ObjectCaptureSession
-  beginNewScanPass() 

Instance Method

# beginNewScanPass()

Resets the state of the capture dial such that the user will need to perform another complete scan pass to fill it and generate a new event in the published property userCompletedScanPass.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func beginNewScanPass()
```

## Discussion

This is intended to be used once the user has completed one scan pass and another scan pass at a different height is desired *without flipping the object*. The same object selection box chosen previously is used, so no new box is chosen. This call is particularly useful for the case where the object is not flippable but multiple passes at different heights are needed to fully capture the object.

This call will throw if the session is not in `.capturing` state (or `.paused` from `.capturing` state).

Note: If the object is flipped and a new scan pass is required, beginNewScanPassAfterFlip() should be called.

Calling this function is only valid in object-centric scanning.

