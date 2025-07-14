

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soVolume 

Global Variable

# soVolume

macOS 10.0+

``` source
var soVolume: OSType { get }
```

## Discussion

Get or set the speech volume for a speech channel.The `speechInfo` parameteris a pointer to a variable of type `Fixed`.Volumes are expressed in fixed-point units ranging from 0.0 through1.0. A value of 0.0 corresponds to silence, and a value of 1.0 correspondsto the maximum possible volume. Volume units lie on a scale thatis linear with amplitude or voltage. A doubling of perceived loudnesscorresponds to a doubling of the volume.

This selector works with both the `GetSpeechInfo` and `SetSpeechInfo` functions.

