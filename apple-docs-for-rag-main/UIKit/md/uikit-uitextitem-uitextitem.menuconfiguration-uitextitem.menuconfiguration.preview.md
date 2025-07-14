

- UIKit
- UITextItem
- UITextItem.MenuConfiguration
-  UITextItem.MenuConfiguration.Preview 

Enumeration

# UITextItem.MenuConfiguration.Preview

Constants that indicate what type of preview to display alongside the text item’s menu.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
enum Preview
```

## Topics

### Getting the preview options

case `default`

An option to show the default system preview alongside the text item’s menu.

case view(UIView)

An option to show the view you provide alongside the text item’s menu.

## See Also

### Creating a menu configuration

convenience init(preview: UITextItem.MenuConfiguration.Preview?, menu: UIMenu)

Creates a text item menu configuration with the specified menu and preview.

