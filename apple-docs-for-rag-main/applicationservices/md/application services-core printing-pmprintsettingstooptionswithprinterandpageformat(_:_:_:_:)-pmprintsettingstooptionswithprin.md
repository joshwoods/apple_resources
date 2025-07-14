

- Application Services
- Core Printing
-  PMPrintSettingsToOptionsWithPrinterAndPageFormat(\_:\_:\_:\_:) 

Function

# PMPrintSettingsToOptionsWithPrinterAndPageFormat(\_:\_:\_:\_:)

Converts print settings and page format data into a CUPS options string for a specified printer.

macOS 10.5+

``` source
func PMPrintSettingsToOptionsWithPrinterAndPageFormat(
    _ settings: PMPrintSettings,
    _ printer: PMPrinter,
    _ pageFormat: PMPageFormat?,
    _ options: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`settings`  

The print settings to convert.

`printer`  

The printer to use for converting the print settings. This parameter must not be `NULL`.

`pageFormat`  

The page format to convert, or `NULL` to specify default page format data.

`options`  

A pointer to a C string. On return, a CUPS option string with the specified print settings and page format data, or `NULL` if the data could not be converted. The function allocates storage for the string. You are responsible for freeing the storage.

## Return Value

A result code. See Result Codes.

## Discussion

This function creates a CUPS options string for the destination printer that captures the data in the specified print settings and page format objects. For example, you could pass this string to the function PMWorkflowSubmitPDFWithOptions(_:_:_:_:) to submit a PDF file for workflow processing. You could also use the options string to run a CUPS filter directly.

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

func PMPrintSettingsToOptions(PMPrintSettings, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings into a CUPS options string.

