

- Foundation
- NSAffineTransform
-  transform(\_:) 

Instance Method

# transform(\_:)

Applies the receiver’s transform to the specified size and returns the results.

Mac Catalyst 13.0+macOS 10.0+

``` source
func transform(_ aSize: NSSize) -> NSSize
```

## Parameters 

`aSize`  

The size data to which you want to apply the matrix.

## Return Value

The resulting size after applying the receiver’s transformations.

## Discussion

This method applies the current rotation and scaling factors to `aSize`; it does not apply translation factors. You can think of this method as transforming a vector whose origin is (0, 0) and whose end point is specified by the value in `aSize`. After the rotation and scaling factors are applied, this method effectively returns the end point of the new vector.

This method is useful for transforming delta or distance values when you need to take scaling and rotation factors into account.

## See Also

### Transforming Data and Objects

func transform(NSPoint) -> NSPoint

Applies the receiver’s transform to the specified point and returns the result.

func transform(NSBezierPath) -> NSBezierPath

Creates and returns a new NSBezierPath object with each point in the given path transformed by the receiver.

