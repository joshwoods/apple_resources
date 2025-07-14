

- RealityKit
- AudioResource
- AudioResource.InputMode
-  AudioResource.InputMode.spatial Deprecated

Case

# AudioResource.InputMode.spatial

a spatialized with all degrees of freedom. This treats a resource as a mono stream so mixes all its channels to mono

iOS 13.0–16.3DeprecatediPadOS 13.0–16.3DeprecatedMac Catalyst 13.0–16.3DeprecatedmacOS 10.15–13.3Deprecated

``` source
case spatial
```

Deprecated

Use the ChannelAudioComponent, AmbientAudioComponent, or SpatialAudioComponent instead.

## See Also

### Input modes

case nonSpatial

the input channels are mixed to whatever the output format is without any spatialization

Deprecated

case ambient

spatialized but ignores listener translation and only follows listener head rotation

Deprecated

