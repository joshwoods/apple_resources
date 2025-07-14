

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.smallSquare 

Case

# NSButton.BezelStyle.smallSquare

A simple square bezel style that can scale to any size.

macOS

``` source
case smallSquare
```

## Discussion

A square style button (sometimes referred to as a “gradient button”) initiates an action related to a view, like adding or removing rows in a table.

These small square buttons contain symbols or interface icons — not text — and you can configure them to behave like push buttons, toggles, or pop-up buttons. The buttons appear near their associated view — usually within or beneath it — so people know which view the buttons affect.

Prefer using a symbol in a gradient button. SF Symbols provides a wide range of symbols that automatically receive appropriate coloring in their default state and in response to user interaction.

Avoid using labels to introduce gradient buttons. Because gradient buttons are closely connected with a specific view, their purpose is generally clear without the need for descriptive text.

- Swift
- Objective-C

```
let button = NSButton()
button.image = NSImage(systemSymbolName: "plus", accessibilityDescription: "")
button.bezelStyle = .smallSquare
```

```
NSButton *button = [[NSButton alloc] init];
button.image = [NSImage imageWithSystemSymbolName:@"plus" accessibilityDescription:nil];
button.bezelStyle = NSBezelStyleSmallSquare;
```

For design guidance, see Human Interface Guidelines > Buttons.

