

- RealityKit
- USD Assets
- USDZ schemas for AR
-  autoPlay 

Article

# autoPlay

Metadata that specifies whether an animation plays automatically on load.

## Overview

Set the autoPlay metadata on the document’s *stage*, that is, the outermost container for scene description. For more information about setting stage metadata, see UsdStage \> Stage Metadata.

Set a value of `true` to play an animation automatically when the scene loads. If this property is `false`, the animation won’t play on load. If an asset omits the `autoPlay` property, the animation plays on load for backward-compatibility.

To support assets that disable `autoPlay`, an app should provide a way to start the animation. For example, when an asset sets `autoPlay` to `false`, AR Quick Look displays a scrubber and a Play button the user can tap to start the animation.

Reality Composer sets this property to `false` when it exports a USDZ to enforce that only behaviors (Preliminary_Behavior) drive animations.

### Declaration

```
bool autoPlay
```

### Disable automatic animation playback

The following asset demonstrates autoPlay alongside existing animation properties, like `startTimeCode` and `endTimeCode`. Because this asset defines autoPlay as `false`, the runtime doesn’t automatically play the animation after it loads this asset.

```
#usda 1.0
(
    endTimeCode = 300
    startTimeCode = 1
    timeCodesPerSecond = 30
    autoPlay = false
    upAxis = "Y"
)

def Xform "AnimatedModel"
{
    def Xform "body"
    {
        double3 xformOp:translate.timeSamples = { ... }
        uniform token[] xformOpOrder = ["xformOp:translate"]
        ...
    }
    ...
}
```

## See Also

### Animation

playbackMode

Metadata that controls animation idling until a behavior takes over.

