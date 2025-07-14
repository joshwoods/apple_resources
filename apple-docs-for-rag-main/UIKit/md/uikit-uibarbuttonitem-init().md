

- UIKit
- UIBarButtonItem
-  init() 

Initializer

# init()

Initializes the item to its default state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init()
```

## See Also

### Creating items

convenience init(title: String?, image: UIImage?, primaryAction: UIAction?, menu: UIMenu?)

Creates a plain-style item using the specified title, image, primary action, and context menu.

convenience init(title: String?, image: UIImage?, target: AnyObject?, action: Selector?, menu: UIMenu?)

Creates a plain-style item using the specified title, image, target, action, and context menu.

init?(coder: NSCoder)

Creates an item from data in an unarchiver.

