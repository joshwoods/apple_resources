

- SceneKit
-  SCNMatrix4MakeRotation(\_:\_:\_:\_:) 

Function

# SCNMatrix4MakeRotation(\_:\_:\_:\_:)

Returns a matrix describing a rotation transformation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**macOS**

``` source
func SCNMatrix4MakeRotation(
    _ angle: CGFloat,
    _ x: CGFloat,
    _ y: CGFloat,
    _ z: CGFloat
) -> SCNMatrix4
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4MakeRotation(
    _ angle: Float,
    _ x: Float,
    _ y: Float,
    _ z: Float
) -> SCNMatrix4
```

## Parameters 

`angle`  

The amount of rotation, in radians, measured counterclockwise around the rotation axis.

`x`  

The x-component of the rotation axis.

`y`  

The y-component of the rotation axis.

`z`  

The z-component of the rotation axis.

## Return Value

A new rotation matrix.

## See Also

### Creating Transform Matrices

func SCNMatrix4MakeTranslation(Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a translation transformation.

func SCNMatrix4MakeScale(Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a scale transformation.

