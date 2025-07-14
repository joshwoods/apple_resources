

- Application Services
- Core Printing
-  PMSessionDefaultPageFormat(\_:\_:) 

Function

# PMSessionDefaultPageFormat(\_:\_:)

Assigns default parameter values to a page format object used in the specified printing session.

macOS 10.0+

``` source
func PMSessionDefaultPageFormat(
    _ printSession: PMPrintSession,
    _ pageFormat: PMPageFormat
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session for the specified page format object.

`pageFormat`  

The page format object to which you want to assign default values.

## Return Value

A result code. See Result Codes.

## Discussion

You must call the function `PMSessionDefaultPageFormat` between the creation and release of the printing session. See the function PMCreateSession(_:).

## See Also

### Creating and Using Page Format Objects

func PMCreatePageFormat(UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a new page format object.

func PMCreatePageFormatWithPMPaper(UnsafeMutablePointer&lt;PMPageFormat?>, PMPaper) -> OSStatus

Creates a page format object with a specified paper.

func PMCopyPageFormat(PMPageFormat, PMPageFormat) -> OSStatus

Copies the settings from one page format object into another.

func PMSessionValidatePageFormat(PMPrintSession, PMPageFormat, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Updates the values in a page format object and validates them against the current formatting printer.

func PMSessionCreatePageFormatList(PMPrintSession, PMPrinter?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains a list of page format objects, each of which describes a paper size available on the specified printer.

func PMPageFormatCreateDataRepresentation(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a page format object.

func PMPageFormatCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a page format object from a data representation.

