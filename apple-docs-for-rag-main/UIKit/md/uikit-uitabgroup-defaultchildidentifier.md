

- UIKit
- UITabGroup
-  defaultChildIdentifier 

Instance Property

# defaultChildIdentifier

The identifier for the default subitem.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var defaultChildIdentifier: String? { get set }
```

## See Also

### Accessing tabs

var children: [UITab]

The tabs within a tab group.

func tab(forIdentifier: String) -> UITab?

Returns a tab with a matching identifier, if any.

var selectedChild: UITab?

The currently selected tab.

