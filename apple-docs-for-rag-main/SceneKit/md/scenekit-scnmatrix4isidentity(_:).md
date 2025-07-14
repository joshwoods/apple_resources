

- SceneKit
-  SCNMatrix4IsIdentity(\_:) 

Function

# SCNMatrix4IsIdentity(\_:)

Returns a Boolean value that indicates whether the specified matrix is equal to the identity matrix.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4IsIdentity(_ m: SCNMatrix4) -> Bool
```

**macOS**

``` source
func SCNMatrix4IsIdentity(_ m: SCNMatrix4) -> Bool
```

## Parameters 

`m`  

The matrix to be tested.

## Return Value

True if the elements on the matrix’s diagonal are `1.0` and all other elements are `0.0`.

## See Also

### Related Documentation

let SCNMatrix4Identity: SCNMatrix4

The 4 x 4 identity matrix.

### Comparing Matrices

func SCNMatrix4EqualToMatrix4(SCNMatrix4, SCNMatrix4) -> Bool

Returns a Boolean value that indicates whether the corresponding elements of two matrices are equal.

