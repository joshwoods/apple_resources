

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechVolumeProperty 

Global Variable

# kSpeechVolumeProperty

Get or set the speech volume for a speech channel.

macOS 10.5+

``` source
let kSpeechVolumeProperty: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object that specifies the speech channel’s speech volume.

Volumes are expressed in floating-point values ranging from 0.0 through 1.0. A value of 0.0 corresponds to silence, and a value of 1.0 corresponds to the maximum possible volume. Volume units lie on a scale that is linear with amplitude or voltage. A doubling of perceived loudness corresponds to a doubling of the volume.

This property works with the CopySpeechProperty(_:_:_:) and SetSpeechProperty(_:_:_:) functions.

