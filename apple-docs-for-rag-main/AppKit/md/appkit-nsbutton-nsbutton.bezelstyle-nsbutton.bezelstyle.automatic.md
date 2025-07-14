

- AppKit
- NSButton
- NSButton.BezelStyle
-  NSButton.BezelStyle.automatic 

Case

# NSButton.BezelStyle.automatic

The default button style based on the button’s contents and position within the window.

macOS 14.0+

``` source
case automatic
```

## Discussion

The system picks which style of button to display automatically based on context and content. This ensures the button displays correctly in toolbars, forms, and touch bar.

In a normal window context, the system picks the NSButton.BezelStyle.push button style. If the system detects that the button has a title that spans multiple lines, or the image content is too tall, it uses NSButton.BezelStyle.flexiblePush.

For design guidance, see Human Interface Guidelines > Buttons.

