

- UIKit
- UILayoutSupport
-  heightAnchor 

Instance Property

# heightAnchor

A layout anchor representing the guide’s height.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var heightAnchor: NSLayoutDimension { get }
```

**Required**

## Discussion

Use this anchor to create constraints with the guide’s height. You can only combine this anchor with other NSLayoutDimension anchors. For more information, see NSLayoutAnchor.

## See Also

### Creating constraints using layout anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the guide’s bottom edge.

**Required**

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the guide’s top edge.

**Required**

