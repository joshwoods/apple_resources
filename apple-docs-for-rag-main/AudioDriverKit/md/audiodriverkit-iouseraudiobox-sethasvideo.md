

- AudioDriverKit
- IOUserAudioBox
-  SetHasVideo 

Instance Method

# SetHasVideo

Sets a Boolean value that indicates the box’s video support.

DriverKit 21.0+

``` source
kern_return_t SetHasVideo(bool in_has_video);
```

## Parameters 

`in_has_video`  

`true` if the box supports video; otherwise, `false`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the video support value sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Determining Media Support

SetHasAudio

Sets a Boolean value that indicates the box’s audio support.

HasAudio

Returns a Boolean value that indicates the box’s audio support.

HasVideo

Returns a Boolean value that indicates the box’s video support.

SetHasMIDI

Sets a Boolean value that indicates the box’s MIDI support.

HasMIDI

Returns a Boolean value that indicates the box’s MIDI support.

