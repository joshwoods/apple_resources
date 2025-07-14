

- AppKit
- NSBezierPath
-  transform(using:) 

Instance Method

# transform(using:)

Transforms all points in the path using the specified transform.

macOS

``` source
func transform(using transform: AffineTransform)
```

## Parameters 

`transform`  

The transform to apply to the path.

## Discussion

This method applies the transform to the path’s points immediately. The following code translates a line from 0,0 to 100,100 to a line from 10,10 to 110,110.

```
NSBezierPath *bezierPath = [NSBezierPath bezierPath];
NSAffineTransform *transform = [NSAffineTransform transform];

[bezierPath moveToPoint: NSMakePoint(0.0, 0.0)];
[bezierPath lineToPoint: NSMakePoint(100.0, 100.0)];

[transform translateXBy: 10.0 yBy: 10.0];
[bezierPath transformUsingAffineTransform: transform];
```

