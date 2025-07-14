

- Application Services
- Core Printing
-  PMPageFormatCreateWithDataRepresentation(\_:\_:) 

Function

# PMPageFormatCreateWithDataRepresentation(\_:\_:)

Creates a page format object from a data representation.

macOS 10.5+

``` source
func PMPageFormatCreateWithDataRepresentation(
    _ data: CFData,
    _ pageFormat: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`data`  

The data representation of a page format object. The data representation must have been previously created with the function PMPageFormatCreateDataRepresentation(_:_:_:).

`pageFormat`  

A pointer to your PMPageFormat variable. On return, the variable refers to a new page format object that contains the information stored in the specified data object. You are responsible for releasing the page format object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## Discussion

This function is typically used to convert a data representation stored in a user document back into a page format object. For information about creating a Core Foundation data object from raw data, see `CFData`.

After calling this function, you should call the function PMSessionValidatePageFormat(_:_:_:) to make sure the page format object contains valid values.

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

func PMPageFormatCreateDataRepresentation(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a page format object.

