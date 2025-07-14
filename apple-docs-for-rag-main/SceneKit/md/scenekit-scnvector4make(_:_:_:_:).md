

- SceneKit
-  SCNVector4Make(\_:\_:\_:\_:) 

Function

# SCNVector4Make(\_:\_:\_:\_:)

Returns a new four-component vector created from individual component values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNVector4Make(
    _ x: Float,
    _ y: Float,
    _ z: Float,
    _ w: Float
) -> SCNVector4
```

**macOS**

``` source
func SCNVector4Make(
    _ x: CGFloat,
    _ y: CGFloat,
    _ z: CGFloat,
    _ w: CGFloat
) -> SCNVector4
```

## Parameters 

`x`  

The first component of the vector.

`y`  

The second component of the vector.

`z`  

The third component of the vector.

`w`  

The fourth component of the vector.

## Return Value

An initialized SCNVector4 structure.

