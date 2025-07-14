

- UIKit
- UITab
-  identifier 

Instance Property

# identifier

A string identifier for a tab.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var identifier: String { get }
```

## Discussion

Each identifier must be unique across all the tabs managed by a UITabBarController.

## See Also

### Accessing a tab’s appearance

var title: String

A tab’s title.

var subtitle: String?

A tab’s subtitle.

var image: UIImage?

A tab’s image.

var badgeValue: String?

A tab’s badge value.

var viewController: UIViewController?

The view controller that the system presents when someone selects a tab.

