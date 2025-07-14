

- SceneKit
-  SCNMatrix4Rotate(\_:\_:\_:\_:\_:) 

Function

# SCNMatrix4Rotate(\_:\_:\_:\_:\_:)

Returns a new matrix created by concatenating the specified matrix with a rotation transformation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4Rotate(
    _ m: SCNMatrix4,
    _ angle: Float,
    _ x: Float,
    _ y: Float,
    _ z: Float
) -> SCNMatrix4
```

**macOS**

``` source
func SCNMatrix4Rotate(
    _ m: SCNMatrix4,
    _ angle: CGFloat,
    _ x: CGFloat,
    _ y: CGFloat,
    _ z: CGFloat
) -> SCNMatrix4
```

## Parameters 

`m`  

The matrix to be combined with a rotation.

`angle`  

The amount of rotation, in radians, measured counterclockwise around the rotation axis.

`x`  

The x-component of the rotation axis.

`y`  

The y-component of the rotation axis.

`z`  

The z-component of the rotation axis.

## Return Value

A new matrix.

## Discussion

The resulting transformation consists of the specified rotation followed by the transformation represented by the `mat` parameter.

## See Also

### Performing Matrix Operations

func SCNMatrix4Translate(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a translation transformation.

func SCNMatrix4Scale(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a scale transformation.

func SCNMatrix4Invert(SCNMatrix4) -> SCNMatrix4

Returns the inverse of the specified matrix.

func SCNMatrix4Mult(SCNMatrix4, SCNMatrix4) -> SCNMatrix4

Returns the product of two matrices.

