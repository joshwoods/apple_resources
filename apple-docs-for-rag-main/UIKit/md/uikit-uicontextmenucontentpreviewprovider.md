

- UIKit
-  UIContextMenuContentPreviewProvider 

Type Alias

# UIContextMenuContentPreviewProvider

Returns the custom view controller to use when previewing your content.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
typealias UIContextMenuContentPreviewProvider = () -> UIViewController?
```

## Return Value

The view controller to display in place of the system’s standard view controller. If you want UIKit to present your content using a default view controller, return `nil`.

## Discussion

Use this handler to load or create your custom view controller, configure it with your content, and return it to UIKit.

## See Also

### Creating the menu configuration object

convenience init(identifier: (any NSCopying)?, previewProvider: UIContextMenuContentPreviewProvider?, actionProvider: UIContextMenuActionProvider?)

Creates a menu configuration object with the specified action and preview providers.

typealias UIContextMenuActionProvider

Returns an action-based contextual menu, optionally incorporating the system-suggested actions.

