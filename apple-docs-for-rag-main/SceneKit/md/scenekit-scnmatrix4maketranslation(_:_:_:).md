

- SceneKit
-  SCNMatrix4MakeTranslation(\_:\_:\_:) 

Function

# SCNMatrix4MakeTranslation(\_:\_:\_:)

Returns a matrix describing a translation transformation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4MakeTranslation(
    _ tx: Float,
    _ ty: Float,
    _ tz: Float
) -> SCNMatrix4
```

**macOS**

``` source
func SCNMatrix4MakeTranslation(
    _ tx: CGFloat,
    _ ty: CGFloat,
    _ tz: CGFloat
) -> SCNMatrix4
```

## Parameters 

`tx`  

The translation distance in the x-axis direction.

`ty`  

The translation distance in the y-axis direction.

`tz`  

The translation distance in the z-axis direction.

## Return Value

A new translation matrix.

## See Also

### Creating Transform Matrices

func SCNMatrix4MakeRotation(Float, Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a rotation transformation.

func SCNMatrix4MakeScale(Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a scale transformation.

