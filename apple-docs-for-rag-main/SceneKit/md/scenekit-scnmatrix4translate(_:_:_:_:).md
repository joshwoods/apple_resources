

- SceneKit
-  SCNMatrix4Translate(\_:\_:\_:\_:) 

Function

# SCNMatrix4Translate(\_:\_:\_:\_:)

Returns a new matrix created by concatenating the specified matrix with a translation transformation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
func SCNMatrix4Translate(
    _ m: SCNMatrix4,
    _ tx: CGFloat,
    _ ty: CGFloat,
    _ tz: CGFloat
) -> SCNMatrix4
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4Translate(
    _ m: SCNMatrix4,
    _ tx: Float,
    _ ty: Float,
    _ tz: Float
) -> SCNMatrix4
```

## Parameters 

`m`  

The matrix to be combined with a translation.

`tx`  

The translation distance in the x-axis direction.

`ty`  

The translation distance in the y-axis direction.

`tz`  

The translation distance in the z-axis direction.

## Return Value

A new matrix.

## Discussion

The resulting transformation consists of the specified translation followed by the transformation represented by the `mat` parameter.

## See Also

### Performing Matrix Operations

func SCNMatrix4Rotate(SCNMatrix4, Float, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a rotation transformation.

func SCNMatrix4Scale(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a scale transformation.

func SCNMatrix4Invert(SCNMatrix4) -> SCNMatrix4

Returns the inverse of the specified matrix.

func SCNMatrix4Mult(SCNMatrix4, SCNMatrix4) -> SCNMatrix4

Returns the product of two matrices.

