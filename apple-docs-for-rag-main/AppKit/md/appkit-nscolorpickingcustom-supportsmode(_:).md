

- AppKit
- NSColorPickingCustom
-  supportsMode(\_:) 

Instance Method

# supportsMode(\_:)

Returns a Boolean value indicating whether or not the receiver supports the specified picking mode.

macOS

``` source
@MainActor
func supportsMode(_ mode: NSColorPanel.Mode) -> Bool
```

**Required**

## Parameters 

`mode`  

The color picking mode.

## Return Value

true if the color picker supports the specified color picking mode; otherwise false.

## Discussion

This method is invoked when the `NSColorPanel` is first initialized: It is used to attempt to restore the user’s previously selected mode. It is also invoked by `NSColorPanel`‘s mode method to find the color picker that supports a particular mode. See this protocol description’s list of the unique mode values for the standard color pickers used by the Application Kit.

## See Also

### Getting Color Picker Information

func currentMode() -> NSColorPanel.Mode

Returns the receiver’s current mode (or submode, if applicable).

**Required**

