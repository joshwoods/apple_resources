

- SceneKit
-  SCNVector3Make(\_:\_:\_:) 

Function

# SCNVector3Make(\_:\_:\_:)

Returns a new three-component vector created from individual component values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
func SCNVector3Make(
    _ x: CGFloat,
    _ y: CGFloat,
    _ z: CGFloat
) -> SCNVector3
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNVector3Make(
    _ x: Float,
    _ y: Float,
    _ z: Float
) -> SCNVector3
```

## Parameters 

`x`  

The first component of the vector.

`y`  

The second component of the vector.

`z`  

The third component of the vector.

## Return Value

An initialized SCNVector3 structure.

