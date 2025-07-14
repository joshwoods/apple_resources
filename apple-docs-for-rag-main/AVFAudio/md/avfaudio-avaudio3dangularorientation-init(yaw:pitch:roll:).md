

- AVFAudio
- AVAudio3DAngularOrientation
-  init(yaw:pitch:roll:) 

Initializer

# init(yaw:pitch:roll:)

Creates a 3D angular orientation using the yaw, pitch, and roll values you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    yaw: Float,
    pitch: Float,
    roll: Float
)
```

## Parameters 

`yaw`  

The side-to-side movement of the listener’s head.

`pitch`  

The up-and-down movement of the listener’s head.

`roll`  

The tilt of the listener’s head.

## See Also

### Creating an Angular Orientation

init()

Creates an angular orientation.

func AVAudioMake3DAngularOrientation(Float, Float, Float) -> AVAudio3DAngularOrientation

Creates a 3D angular orientation using the yaw, pitch, and roll values you specify.

