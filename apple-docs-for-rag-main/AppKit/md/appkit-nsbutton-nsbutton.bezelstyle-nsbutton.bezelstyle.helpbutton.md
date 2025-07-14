

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.helpButton 

Case

# NSButton.BezelStyle.helpButton

A round button with a question mark, providing the standard help button look.

macOS

``` source
case helpButton
```

## Discussion

A help button appears within a view and opens app-specific help documentation.

These are circular, consistently sized buttons that contain a question mark.

- Swift
- Objective-C

```
let button = NSButton()
button.title = ""
button.bezelStyle = .helpButton
```

```
NSButton *button = [[NSButton alloc] init];
button.title = @"";
button.bezelStyle = NSBezelStyleHelpButton;
```

Use the system-provided help button to display your help documentation. People are familiar with the appearance of the standard help button and know that choosing it opens help content.

Include no more than one help button per window. Multiple help buttons in the same context make it hard for people to predict the result of clicking one.

Avoid displaying text that introduces a help button. People know what a help button does, so they don’t need additional descriptive text.

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Informational

case badge

A button style suitable for displaying additional information.

case circular

A round button that can contain either a single character or an icon.

