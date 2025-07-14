

- Application Services
- Core Printing
-  PMSessionCreatePageFormatList(\_:\_:\_:) 

Function

# PMSessionCreatePageFormatList(\_:\_:\_:)

Obtains a list of page format objects, each of which describes a paper size available on the specified printer.

macOS 10.1+

``` source
func PMSessionCreatePageFormatList(
    _ printSession: PMPrintSession,
    _ printer: PMPrinter?,
    _ pageFormatList: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSession`  

The current printing session.

`printer`  

The printer whose list of page sizes you want to enumerate.

`pageFormatList`  

A pointer to your CFArray variable. On return, the variable refers to a Core Foundation array that contains the page format (`PMPageFormat`) objects associated with the specified printer. You are responsible for releasing the array. Each page format object describes a paper size available for the specified printer. If the function fails, then on return the array is `NULL`.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

You can use this function to find the available sheet sizes (and the imageable area for them) for a given printer. After you obtain the page format list, you can call the function PMGetUnadjustedPaperRect(_:_:) for each page format object in the list to obtain the sheet rectangle size. Once you find the paper size you want, call PMGetUnadjustedPageRect(_:_:) to obtain the imageable area for that paper size.

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

func PMPageFormatCreateDataRepresentation(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a page format object.

func PMPageFormatCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a page format object from a data representation.

