

- Matter
- MTRBaseClusterMediaPlayback
-  deactivateTextTrack(with:completion:) 

Instance Method

# deactivateTextTrack(with:completion:)

Command DeactivateTextTrack

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func deactivateTextTrack(
    with params: MTRMediaPlaybackClusterDeactivateTextTrackParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func deactivateTextTrack(with params: MTRMediaPlaybackClusterDeactivateTextTrackParams?) async throws
```

## Discussion

If a Text Track is active (i.e. being displayed), upon receipt of this command, the server SHALL stop displaying it.

