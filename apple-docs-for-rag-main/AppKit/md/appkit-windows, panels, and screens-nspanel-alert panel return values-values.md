

- AppKit
- Windows, Panels, and Screens
- NSPanel
-  Alert Panel Return Values 

API Collection

# Alert Panel Return Values

These constants define values returned by the NSRunAlertPanel function and by the `NSApplication` method runModalSession(_:) when the modal session is run with an `NSPanel` provided by the NSGetAlertPanel function.

## Topics

### Constants

var NSAlertDefaultReturn: Int

The user pressed the default button.

Deprecated

var NSAlertAlternateReturn: Int

The user pressed the alternate button.

Deprecated

var NSAlertOtherReturn: Int

The user pressed a second alternate button.

Deprecated

var NSAlertErrorReturn: Int

The alert cannot identify the reason it was closed; it may have been closed by an external source or by a button other than those listed above.

Deprecated

## See Also

### Constants

Modal Panel Return Values

These constants define the possible return values for such methods as the `runModal...` methods of the NSOpenPanel class, which tell which button (OK or Cancel) the user has clicked on an open panel.

Style Masks

Constants that specify panel styles.

