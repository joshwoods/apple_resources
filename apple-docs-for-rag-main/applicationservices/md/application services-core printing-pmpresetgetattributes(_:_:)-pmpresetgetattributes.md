

- Application Services
- Core Printing
-  PMPresetGetAttributes(\_:\_:) 

Function

# PMPresetGetAttributes(\_:\_:)

Obtains the attributes of a preset.

macOS 10.3+

``` source
func PMPresetGetAttributes(
    _ preset: PMPreset,
    _ attributes: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`preset`  

The preset whose attributes you want to obtain. You can use the function PMPrinterCopyPresets(_:_:) to obtain the presets for a given printer.

`attributes`  

A pointer to your CFDictionary variable. On return, the variable refers to a Core Foundation dictionary containing the attributes of the specified preset, or `NULL` if the attributes could not be obtained. For more information about these attributes, see the Discussion. You should not release this dictionary without first retaining it.

## Return Value

A result code. See Result Codes.

## Discussion

A preset has associated with it a dictionary containing the preset identifier, the localized name, and a description of the environment for which the preset is intended. In addition to these standard attributes, the preset you specify may contain additional attributes that reflect custom print settings.

## See Also

### Using Printer Presets

func PMPresetCopyName(PMPreset, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the localized name for a preset.

func PMPresetCreatePrintSettings(PMPreset, PMPrintSession, UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a print settings object with settings that correspond to a preset.

