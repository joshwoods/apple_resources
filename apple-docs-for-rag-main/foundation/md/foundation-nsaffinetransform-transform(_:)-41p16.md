

- Foundation
- NSAffineTransform
-  transform(\_:) 

Instance Method

# transform(\_:)

Applies the receiver’s transform to the specified point and returns the result.

Mac Catalyst 13.0+macOS 10.0+

``` source
func transform(_ aPoint: NSPoint) -> NSPoint
```

## Parameters 

`aPoint`  

The point in the current coordinate system to which you want to apply the matrix.

## Return Value

The resulting point after applying the receiver’s transformations.

## See Also

### Transforming Data and Objects

func transform(NSSize) -> NSSize

Applies the receiver’s transform to the specified size and returns the results.

func transform(NSBezierPath) -> NSBezierPath

Creates and returns a new NSBezierPath object with each point in the given path transformed by the receiver.

