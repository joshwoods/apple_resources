

- WebKit JS
- DOMWindow
-  webkitConvertPointFromNodeToPage 

Instance Method

# webkitConvertPointFromNodeToPage

Converts a point from node coordinates of a block element to page coordinates.

Safari Desktop 10.1+Safari Mobile 3.0+

``` source
WebKitPoint webkitConvertPointFromNodeToPage(
    optional Node? node, 
    optional WebKitPoint? p
);
```

## Parameters 

`node`  

The coordinate space for `p`.

`p`  

A point in node coordinates to convert to page coordinates.

## Return Value

A point that is at the same location as `p` but in page coordinates.

## See Also

### Converting Points

webkitConvertPointFromPageToNode

Converts a point from page coordinates to node coordinates.

