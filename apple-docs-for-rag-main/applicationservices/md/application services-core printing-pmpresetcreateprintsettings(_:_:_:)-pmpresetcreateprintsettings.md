

- Application Services
- Core Printing
-  PMPresetCreatePrintSettings(\_:\_:\_:) 

Function

# PMPresetCreatePrintSettings(\_:\_:\_:)

Creates a print settings object with settings that correspond to a preset.

macOS 10.3+

``` source
func PMPresetCreatePrintSettings(
    _ preset: PMPreset,
    _ session: PMPrintSession,
    _ printSettings: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`preset`  

The preset whose settings you want to obtain. You can use the function PMPrinterCopyPresets(_:_:) to obtain the presets for a given printer.

`session`  

The session you use to present the Print dialog.

`printSettings`  

A pointer to your PMPrintSettings variable. On return, the variable refers to a print settings object with settings that correspond to the specified preset. You are responsible for releasing the print settings object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## See Also

### Using Printer Presets

func PMPresetCopyName(PMPreset, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the localized name for a preset.

func PMPresetGetAttributes(PMPreset, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Obtains the attributes of a preset.

