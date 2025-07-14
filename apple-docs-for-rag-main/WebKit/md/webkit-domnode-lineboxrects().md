

- WebKit
- DOMNode
-  lineBoxRects() 

Instance Method

# lineBoxRects()

Returns the rectangles that bound each line of text in the node.

macOS 10.5+

``` source
func lineBoxRects() -> [Any]!
```

## Return Value

An array of rectangles, in which each rectangle represents the bounding box of a line of text in the node.

## See Also

### Obtaining layout rectangles

func boundingBox() -> NSRect

Returns a rectangle that bounds the onscreen rendering of the node.

