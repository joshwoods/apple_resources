

- Application Services
- Core Printing
-  PMPageFormatCreateDataRepresentation(\_:\_:\_:) 

Function

# PMPageFormatCreateDataRepresentation(\_:\_:\_:)

Creates a data representation of a page format object.

macOS 10.5+

``` source
func PMPageFormatCreateDataRepresentation(
    _ pageFormat: PMPageFormat,
    _ data: UnsafeMutablePointer?>,
    _ format: PMDataFormat
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object to convert.

`data`  

A pointer to your CFData variable. On return, the variable refers to a new Core Foundation data object that contains a representation of the specified page format object in the specified data format. You are responsible for releasing the data object.

`format`  

A constant that specifies the format of the data representation. Supported values are:

- `kPMDataFormatXMLDefault` (compatible with all macOS versions)

- `kPMDataFormatXMLMinimal` (approximately 3-5 times smaller; compatible with macOS 10.5 and later)

- `kPMDataFormatXMLCompressed` (approximately 20 times smaller; compatible with macOS 10.5 and later)

See PMDataFormat for a full description of these formats.

## Return Value

A result code. See Result Codes.

## Discussion

This function is typically used to convert a page format object into a data representation suitable for storage in a user document. For information about using a Core Foundation data object, see `CFData`.

Before calling this function, you should call the function PMSessionValidatePageFormat(_:_:_:) to make sure the page format object contains valid values.

## See Also

### Creating and Using Page Format Objects

func PMCreatePageFormat(UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a new page format object.

func PMCreatePageFormatWithPMPaper(UnsafeMutablePointer&lt;PMPageFormat?>, PMPaper) -> OSStatus

Creates a page format object with a specified paper.

func PMCopyPageFormat(PMPageFormat, PMPageFormat) -> OSStatus

Copies the settings from one page format object into another.

func PMSessionDefaultPageFormat(PMPrintSession, PMPageFormat) -> OSStatus

Assigns default parameter values to a page format object used in the specified printing session.

func PMSessionValidatePageFormat(PMPrintSession, PMPageFormat, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Updates the values in a page format object and validates them against the current formatting printer.

func PMSessionCreatePageFormatList(PMPrintSession, PMPrinter?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains a list of page format objects, each of which describes a paper size available on the specified printer.

func PMPageFormatCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a page format object from a data representation.

