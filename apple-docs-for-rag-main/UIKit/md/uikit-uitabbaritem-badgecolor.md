

- UIKit
- UITabBarItem
-  badgeColor 

Instance Property

# badgeColor

The background color of the item’s badge.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var badgeColor: UIColor? { get set }
```

## Discussion

The default value is `nil`. If you don’t specify a value, the item uses systemRed.

## See Also

### Configuring the item’s badge

var badgeValue: String?

The text that the item’s badge displays.

func setBadgeTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Registers text attributes that the badge uses for the specified state.

func badgeTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the badge’s text attributes for the specified state.

