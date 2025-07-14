

- SceneKit
-  SCNMatrix4Invert(\_:) 

Function

# SCNMatrix4Invert(\_:)

Returns the inverse of the specified matrix.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**macOS**

``` source
func SCNMatrix4Invert(_ m: SCNMatrix4) -> SCNMatrix4
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4Invert(_ m: SCNMatrix4) -> SCNMatrix4
```

## Parameters 

`m`  

The matrix to be inverted.

## Return Value

The inverse matrix of the specified matrix, or the original matrix if it is not invertible.

## See Also

### Performing Matrix Operations

func SCNMatrix4Translate(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a translation transformation.

func SCNMatrix4Rotate(SCNMatrix4, Float, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a rotation transformation.

func SCNMatrix4Scale(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a scale transformation.

func SCNMatrix4Mult(SCNMatrix4, SCNMatrix4) -> SCNMatrix4

Returns the product of two matrices.

