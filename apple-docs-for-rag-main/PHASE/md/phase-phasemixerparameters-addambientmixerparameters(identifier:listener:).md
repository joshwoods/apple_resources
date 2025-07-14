

- PHASE
- PHASEMixerParameters
-  addAmbientMixerParameters(identifier:listener:) 

Instance Method

# addAmbientMixerParameters(identifier:listener:)

Adds runtime parameters for an ambient mixer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func addAmbientMixerParameters(
    identifier: String,
    listener: PHASEListener
)
```

## Parameters 

`identifier`  

The name of the spatial submixer.

`listener`  

An object that receives a source audio signal. The mixer orients the sound the listener receives based on its transform.

## See Also

### Positioning and Orienting Audio

func addSpatialMixerParameters(identifier: String, source: PHASESource, listener: PHASEListener)

Adds runtime parameters for a spatial mixer.

