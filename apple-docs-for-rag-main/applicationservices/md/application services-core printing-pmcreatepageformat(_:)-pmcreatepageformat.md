

- Application Services
- Core Printing
-  PMCreatePageFormat(\_:) 

Function

# PMCreatePageFormat(\_:)

Creates a new page format object.

macOS 10.0+

``` source
func PMCreatePageFormat(_ pageFormat: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`pageFormat`  

A pointer to your PMPageFormat variable. On return, the variable refers to a new page format object. You are responsible for releasing the page format object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## Discussion

This function allocates memory for a new page format object in your application’s memory space and sets its reference count to 1. The new page format object is empty and unusable until you call PMSessionDefaultPageFormat(_:_:) or PMCopyPageFormat(_:_:).

## See Also

### Creating and Using Page Format Objects

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

func PMPageFormatCreateDataRepresentation(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a page format object.

func PMPageFormatCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a page format object from a data representation.

