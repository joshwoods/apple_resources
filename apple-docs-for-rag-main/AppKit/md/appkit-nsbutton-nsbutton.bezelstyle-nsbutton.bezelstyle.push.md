

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.push 

Case

# NSButton.BezelStyle.push

A standard push style button.

macOS

``` source
case push
```

## Discussion

Use this style when you want the default button style.

- Swift
- Objective-C

```
// Create a push style button.
let cancelButton = NSButton()
cancelButton.title = "Cancel"
cancelButton.bezelStyle = .push

// Create a push style button.
let saveButton = NSButton()
saveButton.title = "Save"
saveButton.bezelStyle = .push
// Make this the default button.
saveButton.keyEquivalent = "\r"
```

```
// Create a push style button.
NSButton *cancelButton = [[NSButton alloc] init];
cancelButton.title = @"Cancel";
cancelButton.bezelStyle = NSBezelStylePush;

// Create a push style button.
NSButton *saveButton = [[NSButton alloc] init];
saveButton.title = @"Save";
saveButton.bezelStyle = NSBezelStylePush;
// Make this the default button.
saveButton.keyEquivalent = @"/r";
```

For design guidance, see Human Interface Guidelines > Buttons.

## See Also

### Push

case flexiblePush

A push button with a flexible height to accommodate longer text labels or an image.

