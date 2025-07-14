

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.accessoryBarAction 

Case

# NSButton.BezelStyle.accessoryBarAction

A button style that you use for extra actions in an accessory toolbar.

macOS

``` source
case accessoryBarAction
```

## Discussion

Use this style when you need to perform an action on a button that appears in an accessory or scope bar.

- Swift
- Objective-C

```
let button = NSButton()
button.title = "Accessory bar action"
button.bezelStyle = .accessoryBarAction
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"Accessory bar action";
button.bezelStyle = NSBezelStyleAccessoryBarAction;
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Toolbar

case toolbar

A button style that’s appropriate for a toolbar item.

case accessoryBar

A button style that’s typically used in the context of an accessory toolbar for buttons that narrow the focus of a search or other operation.

