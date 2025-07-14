

- SceneKit
-  SCNMatrix4Mult(\_:\_:) 

Function

# SCNMatrix4Mult(\_:\_:)

Returns the product of two matrices.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4Mult(
    _ a: SCNMatrix4,
    _ b: SCNMatrix4
) -> SCNMatrix4
```

**macOS**

``` source
func SCNMatrix4Mult(
    _ a: SCNMatrix4,
    _ b: SCNMatrix4
) -> SCNMatrix4
```

## Parameters 

`a`  

The multiplicand, or left operand of matrix multiplication.

`b`  

The multiplier, or right operand of matrix multiplication.

## Return Value

The matrix product of the `matA` and `matB` parameters.

## Discussion

Matrix multiplication is not commutative. As a transformation, the result of multiplying a matrix `A` by a matrix `B` is the transformation represented by `B` followed by the transformation represented by `A`.

## See Also

### Performing Matrix Operations

func SCNMatrix4Translate(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a translation transformation.

func SCNMatrix4Rotate(SCNMatrix4, Float, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a rotation transformation.

func SCNMatrix4Scale(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a scale transformation.

func SCNMatrix4Invert(SCNMatrix4) -> SCNMatrix4

Returns the inverse of the specified matrix.

