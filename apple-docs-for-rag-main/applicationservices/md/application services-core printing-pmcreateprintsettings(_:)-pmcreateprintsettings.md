

- Application Services
- Core Printing
-  PMCreatePrintSettings(\_:) 

Function

# PMCreatePrintSettings(\_:)

Creates a new print settings object.

macOS 10.0+

``` source
func PMCreatePrintSettings(_ printSettings: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`printSettings`  

A pointer to your PMPrintSettings variable. On return, the variable refers to a new print settings object. You are responsible for releasing the print settings object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## Discussion

This function allocates memory for a new print settings object in your application’s memory space and sets its reference count to 1. The new print settings object is empty and unusable until you call PMSessionDefaultPrintSettings(_:_:) or PMCopyPrintSettings(_:_:).

## See Also

### Creating and Using Print Settings Objects

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

func PMPrintSettingsToOptions(PMPrintSettings, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings into a CUPS options string.

func PMPrintSettingsToOptionsWithPrinterAndPageFormat(PMPrintSettings, PMPrinter, PMPageFormat?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings and page format data into a CUPS options string for a specified printer.

