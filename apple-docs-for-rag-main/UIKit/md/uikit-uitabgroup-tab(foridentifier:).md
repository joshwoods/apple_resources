

- UIKit
- UITabGroup
-  tab(forIdentifier:) 

Instance Method

# tab(forIdentifier:)

Returns a tab with a matching identifier, if any.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
func tab(forIdentifier identifier: String) -> UITab?
```

## See Also

### Accessing tabs

var children: [UITab]

The tabs within a tab group.

var defaultChildIdentifier: String?

The identifier for the default subitem.

var selectedChild: UITab?

The currently selected tab.

