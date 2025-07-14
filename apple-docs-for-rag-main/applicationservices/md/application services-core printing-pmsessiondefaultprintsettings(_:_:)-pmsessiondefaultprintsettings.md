

- Application Services
- Core Printing
-  PMSessionDefaultPrintSettings(\_:\_:) 

Function

# PMSessionDefaultPrintSettings(\_:\_:)

Assigns default parameter values to a print settings object for the specified printing session.

macOS 10.0+

``` source
func PMSessionDefaultPrintSettings(
    _ printSession: PMPrintSession,
    _ printSettings: PMPrintSettings
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session for the specified print settings object.

`printSettings`  

The print settings object to which you want to assign default values.

## Return Value

A result code. See Result Codes.

## Discussion

You must call the function `PMSessionDefaultPrintSettings` between the creation and release of a printing session. See the function PMCreateSession(_:).

## See Also

### Creating and Using Print Settings Objects

func PMCreatePrintSettings(UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a new print settings object.

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

