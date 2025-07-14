

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.pushDisclosure 

Case

# NSButton.BezelStyle.pushDisclosure

A bezel style push button with a disclosure triangle.

macOS

``` source
case pushDisclosure
```

## Discussion

Use this style of button when you want your button to look like a disclosure button, commonly seen in toolbars on macOS.

- Swift
- Objective-C

```
let button = NSButton()
button.title = ""
button.bezelStyle = .pushDisclosure
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"";
button.bezelStyle = NSBezelStylePushDisclosure;
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Disclosure

case disclosure

A bezel style button for use with a disclosure triangle.

