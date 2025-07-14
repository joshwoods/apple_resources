

- SceneKit
-  SCNMatrix4MakeScale(\_:\_:\_:) 

Function

# SCNMatrix4MakeScale(\_:\_:\_:)

Returns a matrix describing a scale transformation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
func SCNMatrix4MakeScale(
    _ sx: CGFloat,
    _ sy: CGFloat,
    _ sz: CGFloat
) -> SCNMatrix4
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4MakeScale(
    _ sx: Float,
    _ sy: Float,
    _ sz: Float
) -> SCNMatrix4
```

## Parameters 

`sx`  

The scale factor in the x-axis direction.

`sy`  

The scale factor in the y-axis direction.

`sz`  

The scale factor in the z-axis direction.

## Return Value

A new scale matrix.

## See Also

### Creating Transform Matrices

func SCNMatrix4MakeTranslation(Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a translation transformation.

func SCNMatrix4MakeRotation(Float, Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a rotation transformation.

