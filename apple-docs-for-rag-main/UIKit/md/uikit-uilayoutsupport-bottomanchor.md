

- UIKit
- UILayoutSupport
-  bottomAnchor 

Instance Property

# bottomAnchor

A layout anchor representing the guide’s bottom edge.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var bottomAnchor: NSLayoutYAxisAnchor { get }
```

**Required**

## Discussion

Use this anchor to create constraints with the guide’s bottom edge. You can only combine this anchor with other NSLayoutYAxisAnchor anchors. For more information, see NSLayoutAnchor.

## See Also

### Creating constraints using layout anchors

var heightAnchor: NSLayoutDimension

A layout anchor representing the guide’s height.

**Required**

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the guide’s top edge.

**Required**

