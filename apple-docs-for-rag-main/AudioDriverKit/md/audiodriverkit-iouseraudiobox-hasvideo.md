

- AudioDriverKit
- IOUserAudioBox
-  HasVideo 

Instance Method

# HasVideo

Returns a Boolean value that indicates the box’s video support.

DriverKit 21.0+

``` source
bool HasVideo();
```

## Return Value

`true` if the box supports audio; `false` otherwise.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Determining Media Support

SetHasAudio

Sets a Boolean value that indicates the box’s audio support.

HasAudio

Returns a Boolean value that indicates the box’s audio support.

SetHasVideo

Sets a Boolean value that indicates the box’s video support.

SetHasMIDI

Sets a Boolean value that indicates the box’s MIDI support.

HasMIDI

Returns a Boolean value that indicates the box’s MIDI support.

