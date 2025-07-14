

- UIKit
- UILayoutGuide
-  identifier 

Instance Property

# identifier

A string used to identify the layout guide.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var identifier: String { get set }
```

## Discussion

By default, the `identifier` property is an empty string. Assign a nonempty string to identify this layout guide. This string appears as part of the guide’s description when the guide is printed to the console. You can also use the identifier to find a particular layout guide from among the guides owned by a view.

Identifiers starting with “NS” or “UI” are reserved by the system. The system may assign these identifiers to the guides it creates.

## See Also

### Working with layout guides

var layoutFrame: CGRect

The layout guide’s frame in its owning view’s coordinate system.

var owningView: UIView?

The view that owns this layout guide.

