

- Application Services
- Core Printing
-  PMCopyPageFormat(\_:\_:) 

Function

# PMCopyPageFormat(\_:\_:)

Copies the settings from one page format object into another.

macOS 10.0+

``` source
func PMCopyPageFormat(
    _ formatSrc: PMPageFormat,
    _ formatDest: PMPageFormat
) -> OSStatus
```

## Parameters 

`formatSrc`  

The page format object to duplicate.

`formatDest`  

The page format object to receive the copied settings. On return, this object contains the same settings as the `formatSrc` object.

## Return Value

A result code. See Result Codes.

## See Also

### Creating and Using Page Format Objects

func PMCreatePageFormat(UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a new page format object.

func PMCreatePageFormatWithPMPaper(UnsafeMutablePointer&lt;PMPageFormat?>, PMPaper) -> OSStatus

Creates a page format object with a specified paper.

func PMSessionDefaultPageFormat(PMPrintSession, PMPageFormat) -> OSStatus

Assigns default parameter values to a page format object used in the specified printing session.

func PMSessionValidatePageFormat(PMPrintSession, PMPageFormat, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Updates the values in a page format object and validates them against the current formatting printer.

func PMSessionCreatePageFormatList(PMPrintSession, PMPrinter?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains a list of page format objects, each of which describes a paper size available on the specified printer.

func PMPageFormatCreateDataRepresentation(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a page format object.

func PMPageFormatCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a page format object from a data representation.

