

- Core Animation
- CALayer
-  convertTime(\_:from:) 

Instance Method

# convertTime(\_:from:)

Converts the time interval from the specified layer’s time space to the receiver’s time space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func convertTime(
    _ t: CFTimeInterval,
    from l: CALayer?
) -> CFTimeInterval
```

## Parameters 

`t`  

A point specifying a location in the coordinate system of `l`.

`l`  

The layer with `t` in its time space. The receiver and `l` and must share a common parent layer.

## Return Value

The time interval converted to the receiver’s time space.

## Discussion

The following code shows the creation of two layers, layer and `offsetSlowMoLayer`. `offsetSlowMoLayer` has an offset time of 1 second and its speed is set to `0.5`. The last line converts and prints a time interval of 0.5 seconds converted from the time space of `layer` to the time space of `offsetSlowMoLayer`.

```
let layer = CALayer()
let offsetSlowMoLayer = CALayer()

offsetSlowMoLayer.timeOffset = CFTimeInterval(1)
offsetSlowMoLayer.speed = 0.5

print(offsetSlowMoLayer.convertTime(CFTimeInterval(0.5), from: layer)) // prints 1.25
```

## See Also

### Mapping Between Coordinate and Time Spaces

func convert(CGPoint, from: CALayer?) -> CGPoint

Converts the point from the specified layer’s coordinate system to the receiver’s coordinate system.

func convert(CGPoint, to: CALayer?) -> CGPoint

Converts the point from the receiver’s coordinate system to the specified layer’s coordinate system.

func convert(CGRect, from: CALayer?) -> CGRect

Converts the rectangle from the specified layer’s coordinate system to the receiver’s coordinate system.

func convert(CGRect, to: CALayer?) -> CGRect

Converts the rectangle from the receiver’s coordinate system to the specified layer’s coordinate system.

func convertTime(CFTimeInterval, to: CALayer?) -> CFTimeInterval

Converts the time interval from the receiver’s time space to the specified layer’s time space

