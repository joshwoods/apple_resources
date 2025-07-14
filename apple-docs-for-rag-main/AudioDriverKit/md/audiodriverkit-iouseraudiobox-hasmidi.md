

- AudioDriverKit
- IOUserAudioBox
-  HasMIDI 

Instance Method

# HasMIDI

Returns a Boolean value that indicates the box’s MIDI support.

DriverKit 21.0+

``` source
bool HasMIDI();
```

## Return Value

`true` if the box supports MIDI; `false` otherwise.

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

HasVideo

Returns a Boolean value that indicates the box’s video support.

SetHasMIDI

Sets a Boolean value that indicates the box’s MIDI support.

