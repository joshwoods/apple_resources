

- AppKit
- NSBezierPath
-  clip(\_:) 

Type Method

# clip(\_:)

Intersects the specified rectangle with the clipping path of the current graphics context and makes the resulting shape the current clipping path.

macOS

``` source
class func clip(_ rect: NSRect)
```

## Parameters 

`rect`  

The rectangle to intersect with the current clipping path.

## See Also

### Specifying a Clipping Path

func addClip()

Intersects the area enclosed by the path with the clipping path of the current graphics context and makes the resulting shape the current clipping path.

func setClip()

Replaces the clipping path of the current graphics context with the area inside the path.

