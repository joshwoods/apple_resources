

- Application Services
- Core Printing
-  PMPrintSettingsToOptions(\_:\_:) 

Function

# PMPrintSettingsToOptions(\_:\_:)

Converts print settings into a CUPS options string.

macOS 10.3+

``` source
func PMPrintSettingsToOptions(
    _ settings: PMPrintSettings,
    _ options: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`settings`  

The print settings to convert.

`options`  

A pointer to a C string. On return, a CUPS options string describing the print settings, or `NULL` if the print settings could not be converted. The function allocates storage for the string. You are responsible for freeing the storage.

## Return Value

A result code. See Result Codes.

## Discussion

This function creates a CUPS options string that captures the data in the specified print settings object. In macOS 10.5 and later, Apple recommends that you use the PMPrintSettingsToOptionsWithPrinterAndPageFormat(_:_:_:_:) function instead.

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

func PMCopyPrintSettings(PMPrintSettings, PMPrintSettings) -> OSStatus

Copies the settings from one print settings object into another.

func PMPrintSettingsToOptionsWithPrinterAndPageFormat(PMPrintSettings, PMPrinter, PMPageFormat?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings and page format data into a CUPS options string for a specified printer.

