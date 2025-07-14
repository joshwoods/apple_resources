

- UIKit
- UITabBarItem
-  badgeValue 

Instance Property

# badgeValue

The text that the item’s badge displays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var badgeValue: String? { get set }
```

## Discussion

The default value is `nil`.

## See Also

### Configuring the item’s badge

var badgeColor: UIColor?

The background color of the item’s badge.

func setBadgeTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Registers text attributes that the badge uses for the specified state.

func badgeTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the badge’s text attributes for the specified state.

