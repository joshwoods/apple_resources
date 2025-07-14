

- RealityKit
- AudioResource
- AudioResource.Calibration
-  absolute(dBSPL:) 

Type Method

# absolute(dBSPL:)

The reference level (-12dBLUFS) of the audio source material will be reproduced at the given `dBSPL` level on known audio output hardware.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static func absolute(dBSPL: Audio.Decibel) -> AudioResource.Calibration
```

## Discussion

Note

The -12dBLUFS reference level is achieved automatically by using `Normalization.dynamic`.

