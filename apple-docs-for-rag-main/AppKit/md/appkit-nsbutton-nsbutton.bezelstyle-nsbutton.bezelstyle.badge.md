

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.badge 

Case

# NSButton.BezelStyle.badge

A button style suitable for displaying additional information.

macOS 10.7+

``` source
case badge
```

## Discussion

Use this style of button when you need to provide additional information about something. For example, the count of an item.

- Swift
- Objective-C

```
let button = NSButton()
button.title = "Badge"
button.bezelStyle = .badge
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"Badge";
button.bezelStyle = NSBezelStyleBadge;
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Informational

case helpButton

A round button with a question mark, providing the standard help button look.

case circular

A round button that can contain either a single character or an icon.

