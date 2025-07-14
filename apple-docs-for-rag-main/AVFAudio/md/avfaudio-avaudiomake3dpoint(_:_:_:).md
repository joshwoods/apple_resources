

- AVFAudio
-  AVAudioMake3DPoint(\_:\_:\_:) 

Function

# AVAudioMake3DPoint(\_:\_:\_:)

Creates a 3D point using the x, y, and z coordinates you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func AVAudioMake3DPoint(
    _ x: Float,
    _ y: Float,
    _ z: Float
) -> AVAudio3DPoint
```

## Parameters 

`x`  

The location on the x-axis, in meters.

`y`  

The location on the y-axis, in meters.

`z`  

The location on the z-axis, in meters.

## Return Value

A new AVAudio3DPoint instance.

## See Also

### Creating a Point

init()

Creates a 3D point.

init(x: Float, y: Float, z: Float)

Creates a 3D point using the x, y, and z coordinates you specify.

