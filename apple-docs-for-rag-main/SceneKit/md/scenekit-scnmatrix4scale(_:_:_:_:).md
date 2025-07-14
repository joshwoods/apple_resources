

- SceneKit
-  SCNMatrix4Scale(\_:\_:\_:\_:) 

Function

# SCNMatrix4Scale(\_:\_:\_:\_:)

Returns a new matrix created by concatenating the specified matrix with a scale transformation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4Scale(
    _ m: SCNMatrix4,
    _ sx: Float,
    _ sy: Float,
    _ sz: Float
) -> SCNMatrix4
```

**macOS**

``` source
func SCNMatrix4Scale(
    _ m: SCNMatrix4,
    _ sx: CGFloat,
    _ sy: CGFloat,
    _ sz: CGFloat
) -> SCNMatrix4
```

## Parameters 

`m`  

The matrix to be combined with a translation.

`sx`  

The scale factor in the x-axis direction.

`sy`  

The scale factor in the y-axis direction.

`sz`  

The scale factor in the z-axis direction.

## Return Value

A new matrix.

## Discussion

The resulting transformation consists of the specified scale followed by the transformation represented by the `mat` parameter.

## See Also

### Performing Matrix Operations

func SCNMatrix4Translate(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a translation transformation.

func SCNMatrix4Rotate(SCNMatrix4, Float, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a rotation transformation.

func SCNMatrix4Invert(SCNMatrix4) -> SCNMatrix4

Returns the inverse of the specified matrix.

func SCNMatrix4Mult(SCNMatrix4, SCNMatrix4) -> SCNMatrix4

Returns the product of two matrices.

