

- UIKit
- UITabGroup
-  children 

Instance Property

# children

The tabs within a tab group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var children: [UITab] { get set }
```

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

## See Also

### Accessing tabs

func tab(forIdentifier: String) -> UITab?

Returns a tab with a matching identifier, if any.

var defaultChildIdentifier: String?

The identifier for the default subitem.

var selectedChild: UITab?

The currently selected tab.

