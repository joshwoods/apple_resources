

- AVFAudio
-  AVAudioMake3DAngularOrientation(\_:\_:\_:) 

Function

# AVAudioMake3DAngularOrientation(\_:\_:\_:)

Creates a 3D angular orientation using the yaw, pitch, and roll values you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func AVAudioMake3DAngularOrientation(
    _ yaw: Float,
    _ pitch: Float,
    _ roll: Float
) -> AVAudio3DAngularOrientation
```

## Parameters 

`yaw`  

The side-to-side movement of the listener’s head.

`pitch`  

The up-and-down movement of the listener’s head.

`roll`  

The tilt of the listener’s head.

## Return Value

A new AVAudio3DAngularOrientation instance.

## See Also

### Creating an Angular Orientation

init()

Creates an angular orientation.

init(yaw: Float, pitch: Float, roll: Float)

Creates a 3D angular orientation using the yaw, pitch, and roll values you specify.

