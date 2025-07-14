

- Application Services
- Core Printing
-  PMPresetCopyName(\_:\_:) 

Function

# PMPresetCopyName(\_:\_:)

Obtains the localized name for a preset.

macOS 10.3+

``` source
func PMPresetCopyName(
    _ preset: PMPreset,
    _ name: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`preset`  

The preset object whose localized name you want to obtain. You can use the function PMPrinterCopyPresets(_:_:) to obtain the presets for a given printer.

`paperID`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string containing the localized name of the specified preset. You are responsible for releasing the string.

## Return Value

A result code. See Result Codes.

## See Also

### Using Printer Presets

func PMPresetCreatePrintSettings(PMPreset, PMPrintSession, UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a print settings object with settings that correspond to a preset.

func PMPresetGetAttributes(PMPreset, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Obtains the attributes of a preset.

