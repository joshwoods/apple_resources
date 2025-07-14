

- AppKit
- NSColorPickingCustom
-  currentMode() 

Instance Method

# currentMode()

Returns the receiver’s current mode (or submode, if applicable).

macOS

``` source
@MainActor
func currentMode() -> NSColorPanel.Mode
```

**Required**

## Return Value

The current color picker mode. The returned value should be unique to your color picker. See this protocol description’s list of the unique values for the standard color pickers used by the Application Kit.

## See Also

### Getting Color Picker Information

func supportsMode(NSColorPanel.Mode) -> Bool

Returns a Boolean value indicating whether or not the receiver supports the specified picking mode.

**Required**

