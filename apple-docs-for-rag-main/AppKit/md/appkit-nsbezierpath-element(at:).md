

- AppKit
- NSBezierPath
-  element(at:) 

Instance Method

# element(at:)

Returns the type of path element at the specified index.

macOS

``` source
func element(at index: Int) -> NSBezierPath.ElementType
```

## Parameters 

`index`  

The index of the desired path element.

## Return Value

The type of the path element. For a list of constants, see NSBezierPath.ElementType.

## Discussion

Path elements describe the commands used to define a path and include basic commands such as moving to a specific point, creating a line segment, creating a curve, or closing the path. The elements are stored in the order of their execution.

## See Also

### Related Documentation

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

### Accessing Elements of a Path

var cgPath: CGPath

var elementCount: Int

The total number of path elements in the path.

func element(at: Int, associatedPoints: NSPointArray?) -> NSBezierPath.ElementType

Gets the element type and (and optionally) the associated points for the path element at the specified index.

func removeAllPoints()

Removes all path elements from the path, effectively clearing the path.

func setAssociatedPoints(NSPointArray?, at: Int)

Changes the points associated with the specified path element.

