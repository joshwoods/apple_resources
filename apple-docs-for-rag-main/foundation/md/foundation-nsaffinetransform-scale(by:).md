

- Foundation
- NSAffineTransform
-  scale(by:) 

Instance Method

# scale(by:)

Applies the specified scaling factor along both x and y axes to the receiver’s transformation matrix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func scale(by scale: Double)
```

## Parameters 

`scale`  

The scaling factor to apply to both axes. Specifying a negative value has the effect of inverting the direction of the axes in addition to scaling them. A scaling factor of 1.0 scales the content to exactly the same size.

## Discussion

After invoking this method, applying the receiver’s matrix modifies the unit lengths along the current x and y axes by a factor of `scale`, in addition to performing all previous transformations.

## See Also

### Accumulating Transformations

func rotate(byDegrees: Double)

Applies a rotation factor (measured in degrees) to the receiver’s transformation matrix.

func rotate(byRadians: Double)

Applies a rotation factor (measured in radians) to the receiver’s transformation matrix.

func scaleX(by: Double, yBy: Double)

Applies scaling factors to each axis of the receiver’s transformation matrix.

func translateX(by: Double, yBy: Double)

Applies the specified translation factors to the receiver’s transformation matrix.

func append(NSAffineTransform)

Appends the specified matrix to the receiver’s matrix.

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

func invert()

Replaces the receiver’s matrix with its inverse matrix.

