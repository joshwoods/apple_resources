

- UIKit
- UILayoutSupport
-  topAnchor 

Instance Property

# topAnchor

A layout anchor representing the guide’s top edge.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var topAnchor: NSLayoutYAxisAnchor { get }
```

**Required**

## Discussion

Use this anchor to create constraints with the guide’s top edge. You can only combine this anchor with other NSLayoutYAxisAnchor anchors. For more information, see NSLayoutAnchor.

## See Also

### Creating constraints using layout anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the guide’s bottom edge.

**Required**

var heightAnchor: NSLayoutDimension

A layout anchor representing the guide’s height.

**Required**

