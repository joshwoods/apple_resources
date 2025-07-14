

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.circular 

Case

# NSButton.BezelStyle.circular

A round button that can contain either a single character or an icon.

macOS

``` source
case circular
```

## Discussion

Use this button type to display either a single character:

- Swift
- Objective-C

```
let button = NSButton()
button.title = "C"
button.bezelStyle = .circular
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"C";
button.bezelStyle = NSBezelStyleCircular;
```

Or a small icon.

- Swift
- Objective-C

```
let button = NSButton()
button.image = NSImage(systemSymbolName: "star", accessibilityDescription: "")
button.bezelStyle = .circular
```

```
NSButton *button = [[NSButton alloc] init];
button.image = [NSImage imageWithSystemSymbolName:@"star" accessibilityDescription:nil];
button.bezelStyle = NSBezelStyleCircular;
```

Use system images such as SF Symbols for best results as they automatically scale to fit the button. Large images don’t clip when they display with this style. Instead, they shrink to fit the button’s bounds.

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Informational

case helpButton

A round button with a question mark, providing the standard help button look.

case badge

A button style suitable for displaying additional information.

