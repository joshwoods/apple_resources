

- AppKit
- NSColor
-  systemColorsDidChangeNotification 

Type Property

# systemColorsDidChangeNotification

Sent when the system colors have changed, such as through a system control panel interface.

macOS

``` source
class let systemColorsDidChangeNotification: NSNotification.Name
```

## Discussion

This notification contains no notification object and no `userInfo` dictionary.

## See Also

### Determining When Colors Change

class let currentControlTintDidChangeNotification: NSNotification.Name

Sent after the user changes control tint preference.

Deprecated

