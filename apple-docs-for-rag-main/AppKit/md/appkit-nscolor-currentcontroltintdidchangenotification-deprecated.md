

- AppKit
- NSColor
-  currentControlTintDidChangeNotification Deprecated

Type Property

# currentControlTintDidChangeNotification

Sent after the user changes control tint preference.

macOS 10.0–11.0Deprecated

``` source
class let currentControlTintDidChangeNotification: NSNotification.Name
```

Deprecated

Changes to the accent color can be manually observed by implementing -viewDidChangeEffectiveAppearance in a NSView subclass, or by Key-Value Observing the -effectiveAppearance property on NSApplication. Views are automatically redisplayed when the accent color changes.

## Discussion

The notification object is `NSApp`. This notification does not contain a `userInfo` dictionary.

## See Also

### Determining When Colors Change

class let systemColorsDidChangeNotification: NSNotification.Name

Sent when the system colors have changed, such as through a system control panel interface.

