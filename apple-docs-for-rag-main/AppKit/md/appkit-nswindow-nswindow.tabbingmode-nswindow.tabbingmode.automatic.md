

- AppKit
- NSWindow
- NSWindow.TabbingMode
-  NSWindow.TabbingMode.automatic 

Case

# NSWindow.TabbingMode.automatic

A window that automatically tabs together based on the user’s tabbing preference.

macOS 10.12+

``` source
case automatic
```

## Discussion

A window with the NSWindow.TabbingMode.automatic tabbing mode consults the value of userTabbingPreference to decide if it should join a tab group with other windows.

## See Also

### Modes

case disallowed

A window that explicitly does not prefer to tab together with other windows.

case preferred

A window that explicitly prefers to tab together with other windows with the same tabbing identifier.

