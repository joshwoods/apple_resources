

- AVFAudio
-  AVAudioMake3DVectorOrientation(\_:\_:) 

Function

# AVAudioMake3DVectorOrientation(\_:\_:)

Creates a 3D vector orientation instance using the forward and up vectors you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func AVAudioMake3DVectorOrientation(
    _ forward: AVAudio3DVector,
    _ up: AVAudio3DVector
) -> AVAudio3DVectorOrientation
```

## Parameters 

`forward`  

The forward vector points in the direction that the listener faces.

`up`  

The up vector is orthogonal to the forward vector and points upward from the listener’s head.

## Return Value

A new AVAudioMake3DVectorOrientation(_:_:) object.

## See Also

### Creating a Vector Orientation

init()

Creates a 3D vector orientation instance.

init(forward: AVAudio3DVector, up: AVAudio3DVector)

Creates a 3D vector orientation instance using the forward and up vectors you specify.

