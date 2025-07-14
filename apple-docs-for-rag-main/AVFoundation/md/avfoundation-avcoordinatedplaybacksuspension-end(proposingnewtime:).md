

- AVFoundation
- AVCoordinatedPlaybackSuspension
-  end(proposingNewTime:) 

Instance Method

# end(proposingNewTime:)

Ends a suspension and proposes a new playback time to the group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func end(proposingNewTime time: CMTime)
```

## Parameters 

`time`  

The proposed playback time. Passing a nonnumeric time results in the same behavior as calling the end() method.

## Discussion

If this is the last suspension, the coordinator proposes a new time to the group without changing the group’s playback rate. If it isn’t, the coordinator only proposes the new time after all other suspensions end.

A suspension that ends after this one ends can override the proposed time. Similarly, playback commands from the group that arrive after this suspension ends, override a pending proposal.

## See Also

### Ending a Suspension

func end()

Ends a suspension.

