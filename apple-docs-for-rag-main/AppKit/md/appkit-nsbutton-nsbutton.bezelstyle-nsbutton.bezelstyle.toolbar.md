

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.toolbar 

Case

# NSButton.BezelStyle.toolbar

A button style that’s appropriate for a toolbar item.

macOS

``` source
case toolbar
```

## Discussion

Use this case for displaying a button in an NSToolbar.

- Swift
- Objective-C

```
let button = NSButton()
button.title = "Toolbar"
button.bezelStyle = .toolbar
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"Toolbar";
button.bezelStyle = NSBezelStyleToolbar;
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Toolbar

case accessoryBar

A button style that’s typically used in the context of an accessory toolbar for buttons that narrow the focus of a search or other operation.

case accessoryBarAction

A button style that you use for extra actions in an accessory toolbar.

