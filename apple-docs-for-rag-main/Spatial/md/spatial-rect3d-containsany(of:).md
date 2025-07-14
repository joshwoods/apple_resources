

- Spatial
- Rect3D
-  containsAny(of:) 

Instance Method

# containsAny(of:)

Returns a Boolean value that indicates whether the rectangle contains any of the specified points.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func containsAny(of points: [Point3D]) -> Bool
```

## Parameters 

`points`  

The array of points that the function compares against.

## Return Value

A Boolean value that indicates whether the rectangle contains any of the specified points.

## See Also

### Deprecated symbols

func distance(to: Rect3D) -> Double

Returns the distance between the origins of two rectangle.

Deprecated

func rotation(to: Rect3D) -> Rotation3D

Returns the rotation around @p (0,0,0) from the first rectangle to the second rectangle.

Deprecated

var maxX: DoubleDeprecated

var maxY: DoubleDeprecated

var maxZ: DoubleDeprecated

var midX: DoubleDeprecated

var midY: DoubleDeprecated

var midZ: DoubleDeprecated

var minX: DoubleDeprecated

var minY: DoubleDeprecated

var minZ: DoubleDeprecated

