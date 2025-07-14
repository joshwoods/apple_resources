

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.accessoryBar 

Case

# NSButton.BezelStyle.accessoryBar

A button style that’s typically used in the context of an accessory toolbar for buttons that narrow the focus of a search or other operation.

macOS

``` source
case accessoryBar
```

## Discussion

Use this style of button to display some kind of toggle or selection state, like a favorites bar or search scope.

- Swift
- Objective-C

```
// Create an accessory bar style button.
let rankButton = NSButton()
rankButton.title = "Search Rank"
rankButton.bezelStyle = .accessoryBar
rankButton.setButtonType(.pushOnPushOff)

// Create an accessory bar style button.
let orderButton = NSButton()
orderButton.title = "Page Order"
orderButton.bezelStyle = .accessoryBar
orderButton.setButtonType(.pushOnPushOff)
```

```
// Create an accessory bar style button.
NSButton *rankButton = [[NSButton alloc] init];
rankButton.title = @"Search Rank";
rankButton.bezelStyle = NSBezelStyleAccessoryBar;
[rankButton setButtonType:NSButtonTypePushOnPushOff];

// Create an accessory bar style button.
NSButton *orderButton = [[NSButton alloc] init];
orderButton.title = @"Page Order";
orderButton.bezelStyle = NSBezelStyleAccessoryBar;
[orderButton setButtonType:NSButtonTypePushOnPushOff];
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Toolbar

case toolbar

A button style that’s appropriate for a toolbar item.

case accessoryBarAction

A button style that you use for extra actions in an accessory toolbar.

