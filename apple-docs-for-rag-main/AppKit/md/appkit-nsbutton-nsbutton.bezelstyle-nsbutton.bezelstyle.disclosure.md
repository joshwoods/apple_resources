

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.disclosure 

Case

# NSButton.BezelStyle.disclosure

A bezel style button for use with a disclosure triangle.

macOS

``` source
case disclosure
```

## Discussion

Use this style of button when you want to reveal more information. When you use this bezel style along with the NSButton.ButtonType.pushOnPushOff button type, the button points it’s disclosure triangle to the right representing a closed state. When someone clicks the button the triangle animates down representing an open state.

- Swift
- Objective-C

```
let button = NSButton()
button.title = ""
button.setButtonType(.pushOnPushOff)
button.bezelStyle = .disclosure
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"";
button.bezelStyle = NSBezelStyleDisclosure;
[button setButtonType:NSButtonTypePushOnPushOff];
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Disclosure

case pushDisclosure

A bezel style push button with a disclosure triangle.

