

- Application Services
- Core Printing
-  PMSessionValidatePageFormat(\_:\_:\_:) 

Function

# PMSessionValidatePageFormat(\_:\_:\_:)

Updates the values in a page format object and validates them against the current formatting printer.

macOS 10.0+

``` source
func PMSessionValidatePageFormat(
    _ printSession: PMPrintSession,
    _ pageFormat: PMPageFormat,
    _ changed: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session for the specified page format object.

`pageFormat`  

The page format object to validate.

`result`  

A pointer to your Boolean variable. On return, `true` if the function set the page format object to default values; otherwise, `false`.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of the printing session. See the function PMCreateSession(_:).

The function `PMSessionValidatePageFormat` validates the page format object against the current formatting printer. The formatting printer is displayed in the Format for pop-up menu in the Page Setup dialog. The default formatting printer is the generic Any Printer. If the page format object contains values that are not valid for the formatting printer, the page format object is set to default values and the `result` parameter is set to `true`.

Validating a page format object also causes calculated fields (such as the adjusted paper and page rectangles) to be updated based on the changed settings (such as resolution, scaling, and page orientation). If the page format object contains values that are valid for the formatting printer but need to be updated, the `result` parameter is set to `false`.

After you call any function that makes changes to a page format object (such as `PMSetOrientation`), you should call the function `PMSessionValidatePageFormat` to validate the page format object before using that object.

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

func PMSessionCreatePageFormatList(PMPrintSession, PMPrinter?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains a list of page format objects, each of which describes a paper size available on the specified printer.

func PMPageFormatCreateDataRepresentation(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, PMDataFormat) -> OSStatus

Creates a data representation of a page format object.

func PMPageFormatCreateWithDataRepresentation(CFData, UnsafeMutablePointer&lt;PMPageFormat?>) -> OSStatus

Creates a page format object from a data representation.

