

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.flexiblePush 

Case

# NSButton.BezelStyle.flexiblePush

A push button with a flexible height to accommodate longer text labels or an image.

macOS

``` source
case flexiblePush
```

## Discussion

Use this style of button when you need to accommodate tall or variable height content.

Tall or variable height content includes text with newlines (\`n\`) as well as buttons you constrain the width of through Auto Layout. This style automatically wraps text based on button width and available space.

- Swift
- Objective-C

```
let button = NSButton()
button.title = "Flexible\n push"
button.bezelStyle = .flexiblePush
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"Flexible\n push";
button.bezelStyle = NSBezelStyleFlexiblePush;
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Push

case push

A standard push style button.

