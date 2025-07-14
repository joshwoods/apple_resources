

- UIKit
- UITabGroup
-  selectedChild 

Instance Property

# selectedChild

The currently selected tab.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var selectedChild: UITab? { get set }
```

## See Also

### Accessing tabs

var children: [UITab]

The tabs within a tab group.

func tab(forIdentifier: String) -> UITab?

Returns a tab with a matching identifier, if any.

var defaultChildIdentifier: String?

The identifier for the default subitem.

