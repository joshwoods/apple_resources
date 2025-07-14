

- AVFAudio
- AVAudio3DVectorOrientation
-  init(forward:up:) 

Initializer

# init(forward:up:)

Creates a 3D vector orientation instance using the forward and up vectors you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    forward: AVAudio3DVector,
    up: AVAudio3DVector
)
```

## Parameters 

`forward`  

The forward vector points in the direction that the listener faces.

`up`  

The up vector is orthogonal to the forward vector and points upward from the listener’s head.

## See Also

### Creating a Vector Orientation

init()

Creates a 3D vector orientation instance.

func AVAudioMake3DVectorOrientation(AVAudio3DVector, AVAudio3DVector) -> AVAudio3DVectorOrientation

Creates a 3D vector orientation instance using the forward and up vectors you specify.

