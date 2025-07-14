

- AVFoundation
- AVCaptureMovieFileOutput
-  recordsVideoOrientationAndMirroringChangesAsMetadataTrack(for:) 

Instance Method

# recordsVideoOrientationAndMirroringChangesAsMetadataTrack(for:)

A Boolean value that indicates whether the movie file output records video orientation and mirroring information as a metadata track.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func recordsVideoOrientationAndMirroringChangesAsMetadataTrack(for connection: AVCaptureConnection) -> Bool
```

## Parameters 

`connection`  

A connection delivering video media to the movie file output. This method throws an invalid argument exception if the value isn’t a video connection or if the connection doesn’t terminate at the movie file output.

## See Also

### Setting orientation

func setRecordsVideoOrientationAndMirroringChangesAsMetadataTrack(Bool, for: AVCaptureConnection)

Sets whether the movie file output creates a timed metadata track to capture changes to the connection’s video orientation and mirroring.

