

- AVFoundation
- AVAssetExportSession
-  audioTrackGroupHandling 

Instance Property

# audioTrackGroupHandling

A policy that defines how the session exports alternate audio tracks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var audioTrackGroupHandling: AVAssetTrackGroupOutputHandling { get set }
```

## Discussion

By default, a session exports only the enabled audio tracks within an alternate track group from the source asset. You can specify that the session preserve all audio tracks within an alternate track group by setting this value to preserveAlternateTracks.

If no audio alternate track group is present, the value of this property has no effect. You can query the trackGroups property of AVAsset to determine whether it contains audio track groups.

Important

You can’t specify alternate track output handling while also setting a value for the export session’s audioMix property. The system throws an exception if you specify both.

## See Also

### Configuring Track Groups

struct AVAssetTrackGroupOutputHandling

A type that specifies policies for how an export session processes alternate tracks in a track group.

