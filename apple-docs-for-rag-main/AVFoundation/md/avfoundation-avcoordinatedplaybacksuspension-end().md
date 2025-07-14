

- AVFoundation
- AVCoordinatedPlaybackSuspension
-  end() 

Instance Method

# end()

Ends a suspension.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func end()
```

## Discussion

If this is the last suspension, the coordinator adjusts the timing of its playback object to match the group.

To end a suspension and simultaneously propose a new playback time to the group, call the end(proposingNewTime:) method.

## See Also

### Ending a Suspension

func end(proposingNewTime: CMTime)

Ends a suspension and proposes a new playback time to the group.

