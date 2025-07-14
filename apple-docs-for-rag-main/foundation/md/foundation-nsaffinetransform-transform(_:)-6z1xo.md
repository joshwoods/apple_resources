

- Foundation
- NSAffineTransform
-  transform(\_:) 

Instance Method

# transform(\_:)

Creates and returns a new NSBezierPath object with each point in the given path transformed by the receiver.

macOS 10.0+

``` source
func transform(_ path: NSBezierPath) -> NSBezierPath
```

## Parameters 

`path`  

An object representing the bezier path to be used in the transformation.

## Discussion

The original `NSBezierPath` object is not modified.

## See Also

### Transforming Data and Objects

func transform(NSPoint) -> NSPoint

Applies the receiver’s transform to the specified point and returns the result.

func transform(NSSize) -> NSSize

Applies the receiver’s transform to the specified size and returns the results.

