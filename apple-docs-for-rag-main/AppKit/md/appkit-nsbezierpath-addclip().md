

- AppKit
- NSBezierPath
-  addClip() 

Instance Method

# addClip()

Intersects the area enclosed by the path with the clipping path of the current graphics context and makes the resulting shape the current clipping path.

macOS

``` source
func addClip()
```

## Discussion

This method uses the current winding rule to determine the clipping shape of the receiver. This method does not affect the receiver’s path.

## See Also

### Specifying a Clipping Path

func setClip()

Replaces the clipping path of the current graphics context with the area inside the path.

class func clip(NSRect)

Intersects the specified rectangle with the clipping path of the current graphics context and makes the resulting shape the current clipping path.

