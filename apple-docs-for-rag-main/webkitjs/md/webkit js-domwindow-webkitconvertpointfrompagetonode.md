

- WebKit JS
- DOMWindow
-  webkitConvertPointFromPageToNode 

Instance Method

# webkitConvertPointFromPageToNode

Converts a point from page coordinates to node coordinates.

Safari Desktop 10.1+Safari Mobile 3.0+

``` source
WebKitPoint webkitConvertPointFromPageToNode(
    optional Node? node, 
    optional WebKitPoint? p
);
```

## Parameters 

`node`  

The coordinate space to convert the given point to.

`p`  

A point in page coordinates to convert to node coordinates.

## Return Value

A point that is at the same location as `p` but in node coordinates.

## See Also

### Converting Points

webkitConvertPointFromNodeToPage

Converts a point from node coordinates of a block element to page coordinates.

