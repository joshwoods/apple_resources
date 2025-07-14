

- Core Animation
- CALayer
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts the rectangle from the specified layer’s coordinate system to the receiver’s coordinate system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func convert(
    _ r: CGRect,
    from l: CALayer?
) -> CGRect
```

## Parameters 

`r`  

A point specifying a location in the coordinate system of `l`.

`l`  

The layer with `r` in its coordinate system. The receiver and `l` and must share a common parent layer. This parameter may be `nil`.

## Return Value

The rectangle converted to the receiver’s coordinate system.

## Discussion

If you specify `nil` for the `l` parameter, this method returns the original rect with an origin subtracted from the layer’s frame’s origin.

The following example shows code that creates two layers, `redLayer` and `yellowLayer`. `yellowLayer` is scaled so that it is half of its original size.

```
let layerFrame = CGRect(x: 0, y: 0, width: 640, height: 480)

let redLayer = CALayer()
redLayer.frame = layerFrame
redLayer.backgroundColor = UIColor.red.cgColor

let yellowLayer = CALayer()
yellowLayer.frame = layerFrame
yellowLayer.backgroundColor = UIColor.yellow.cgColor
yellowLayer.transform = CATransform3DMakeScale(0.5, 0.5, 1)
```

The following figure shows the two layers and an overlaid rectangle with a frame of `(50, 50, 200, 200)` in the red layer’s coordinate system.

The following code shows how you can find the coordinates of that rectangle in the yellow layer’s coordinate system.

```
let rect = CGRect(x: 50, y: 50, width: 200, height: 200)
print(yellowLayer.convert(rect, from: redLayer)) // prints (-220.0, -140.0, 400.0, 400.0)
```

## See Also

### Mapping Between Coordinate and Time Spaces

func convert(CGPoint, from: CALayer?) -> CGPoint

Converts the point from the specified layer’s coordinate system to the receiver’s coordinate system.

func convert(CGPoint, to: CALayer?) -> CGPoint

Converts the point from the receiver’s coordinate system to the specified layer’s coordinate system.

func convert(CGRect, to: CALayer?) -> CGRect

Converts the rectangle from the receiver’s coordinate system to the specified layer’s coordinate system.

func convertTime(CFTimeInterval, from: CALayer?) -> CFTimeInterval

Converts the time interval from the specified layer’s time space to the receiver’s time space.

func convertTime(CFTimeInterval, to: CALayer?) -> CFTimeInterval

Converts the time interval from the receiver’s time space to the specified layer’s time space

