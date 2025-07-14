

- Application Services
- Core Printing
-  PMCopyPrintSettings(\_:\_:) 

Function

# PMCopyPrintSettings(\_:\_:)

Copies the settings from one print settings object into another.

macOS 10.0+

``` source
func PMCopyPrintSettings(
    _ settingSrc: PMPrintSettings,
    _ settingDest: PMPrintSettings
) -> OSStatus
```

## Parameters 

`settingSrc`  

The print settings object to duplicate.

`settingDest`  

The print settings object to receive the copied settings. On return, this object contains the same settings as the `settingSrc` object.

## Return Value

A result code. See Result Codes.

## See Also

### Creating and Using Print Settings Objects

func PMCreatePrintSettings(UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a new print settings object.

func PMSessionDefaultPrintSettings(PMPrintSession, PMPrintSettings) -> OSStatus

Assigns default parameter values to a print settings object for the specified printing session.

func PMSessionValidatePrintSettings(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Validates a print settings object within the context of the specified printing session.

func PMPrintSettingsCreateDataRepresentation(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a print settings object.

func PMPrintSettingsCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a print settings object from a data representation.

func PMPrintSettingsToOptions(PMPrintSettings, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings into a CUPS options string.

func PMPrintSettingsToOptionsWithPrinterAndPageFormat(PMPrintSettings, PMPrinter, PMPageFormat?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings and page format data into a CUPS options string for a specified printer.

