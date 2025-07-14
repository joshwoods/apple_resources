

- AppKit
- NSBezierPath
-  removeAllPoints() 

Instance Method

# removeAllPoints()

Removes all path elements from the path, effectively clearing the path.

macOS

``` source
func removeAllPoints()
```

## See Also

### Accessing Elements of a Path

var cgPath: CGPath

var elementCount: Int

The total number of path elements in the path.

func element(at: Int) -> NSBezierPath.ElementType

Returns the type of path element at the specified index.

func element(at: Int, associatedPoints: NSPointArray?) -> NSBezierPath.ElementType

Gets the element type and (and optionally) the associated points for the path element at the specified index.

func setAssociatedPoints(NSPointArray?, at: Int)

Changes the points associated with the specified path element.

