

- Application Services
- Core Printing
-  PMCreatePageFormatWithPMPaper(\_:\_:) 

Function

# PMCreatePageFormatWithPMPaper(\_:\_:)

Creates a page format object with a specified paper.

macOS 10.3+

``` source
func PMCreatePageFormatWithPMPaper(
    _ pageFormat: UnsafeMutablePointer,
    _ paper: PMPaper
) -> OSStatus
```

## Parameters 

`pageFormat`  

A pointer to your PMPageFormat variable. On return, the variable refers to a new page format object that represents the specified paper. You are responsible for releasing the page format object with the function PMRelease(_:).

`paper`  

The type of paper for the new page format object.

## Return Value

A result code. See Result Codes.

## See Also

### Creating and Using Page Format Objects

func PMCreatePageFormat(UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a new page format object.

func PMCopyPageFormat(PMPageFormat, PMPageFormat) -> OSStatus

Copies the settings from one page format object into another.

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

