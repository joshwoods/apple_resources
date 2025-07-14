

- AppKit
- NSBezierPath
-  cgPath 

Instance Property

# cgPath

macOS 14.0+

``` source
var cgPath: CGPath { get set }
```

## See Also

### Accessing Elements of a Path

var elementCount: Int

The total number of path elements in the path.

func element(at: Int) -> NSBezierPath.ElementType

Returns the type of path element at the specified index.

func element(at: Int, associatedPoints: NSPointArray?) -> NSBezierPath.ElementType

Gets the element type and (and optionally) the associated points for the path element at the specified index.

func removeAllPoints()

Removes all path elements from the path, effectively clearing the path.

func setAssociatedPoints(NSPointArray?, at: Int)

Changes the points associated with the specified path element.

