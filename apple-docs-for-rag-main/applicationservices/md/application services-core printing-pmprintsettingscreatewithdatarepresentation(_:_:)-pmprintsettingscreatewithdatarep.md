

- Application Services
- Core Printing
-  PMPrintSettingsCreateWithDataRepresentation(\_:\_:) 

Function

# PMPrintSettingsCreateWithDataRepresentation(\_:\_:)

Creates a print settings object from a data representation.

macOS 10.5+

``` source
func PMPrintSettingsCreateWithDataRepresentation(
    _ data: CFData,
    _ printSettings: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`data`  

The data representation of a print settings object. The data representation must have been previously created with the function PMPrintSettingsCreateDataRepresentation(_:_:_:).

`printSettings`  

A pointer to your PMPrintSettings variable. On return, the variable refers to a new print settings object that contains the printing information stored in the specified data object. You are responsible for releasing the print settings object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## Discussion

This function is typically used to convert a data representation stored in a user document back into a print settings object. For information about creating a Core Foundation data object from raw data, see `CFData`.

After calling this function, you should call the function PMSessionValidatePrintSettings(_:_:_:) to make sure the print settings object contains valid values.

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

func PMCopyPrintSettings(PMPrintSettings, PMPrintSettings) -> OSStatus

Copies the settings from one print settings object into another.

func PMPrintSettingsToOptions(PMPrintSettings, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings into a CUPS options string.

func PMPrintSettingsToOptionsWithPrinterAndPageFormat(PMPrintSettings, PMPrinter, PMPageFormat?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Converts print settings and page format data into a CUPS options string for a specified printer.

