

- Application Services
- Core Printing
-  PMPrintSettingsCreateDataRepresentation(\_:\_:\_:) 

Function

# PMPrintSettingsCreateDataRepresentation(\_:\_:\_:)

Creates a data representation of a print settings object.

macOS 10.5+

``` source
func PMPrintSettingsCreateDataRepresentation(
    _ printSettings: PMPrintSettings,
    _ data: UnsafeMutablePointer?>,
    _ format: PMDataFormat
) -> OSStatus
```

## Parameters 

`printSettings`  

The print settings object to convert.

`data`  

A pointer to your CFData variable. On return, the variable refers to a new Core Foundation data object that contains a representation of the specified print settings object in the specified data format. You are responsible for releasing the data object.

`format`  

A constant that specifies the format of the data representation. Supported values are:

- `kPMDataFormatXMLDefault` (compatible with all macOS versions)

- `kPMDataFormatXMLMinimal` (approximately 3-5 times smaller; compatible with macOS 10.5 and later)

- `kPMDataFormatXMLCompressed` (approximately 20 times smaller; compatible with macOS 10.5 and later)

See PMDataFormat for a full description of these formats.

## Return Value

A result code. See Result Codes.

## Discussion

This function is typically used to convert a print settings object into a data representation suitable for storage in a user document. For information about using a Core Foundation data object, see `CFData`.

Before calling this function, you should call the function PMSessionValidatePrintSettings(_:_:_:) to make sure the print settings object contains valid values.

Apple recommends that you do not reuse the print settings information if the user prints the document again. The information supplied by the user in the Print dialog should pertain to the document only while the document prints, so there is no need to save the print settings object.

## See Also

### Creating and Using Print Settings Objects

func PMCreatePrintSettings(UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a new print settings object.

func PMSessionDefaultPrintSettings(PMPrintSession, PMPrintSettings) -> OSStatus

Assigns default parameter values to a print settings object for the specified printing session.

func PMSessionValidatePrintSettings(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Validates a print settings object within the context of the specified printing session.

func PMPrintSettingsCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPrintSettings?>) -> OSStatus

Creates a print settings object from a data representation.

func PMCopyPrintSettings(PMPrintSettings, PMPrintSettings) -> OSStatus

Copies the settings from one print settings object into another.

func PMPrintSettingsToOptions(PMPrintSettings, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings into a CUPS options string.

func PMPrintSettingsToOptionsWithPrinterAndPageFormat(PMPrintSettings, PMPrinter, PMPageFormat?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings and page format data into a CUPS options string for a specified printer.

