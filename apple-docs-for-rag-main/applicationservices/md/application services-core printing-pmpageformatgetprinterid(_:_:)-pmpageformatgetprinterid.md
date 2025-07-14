

- Application Services
- Core Printing
-  PMPageFormatGetPrinterID(\_:\_:) 

Function

# PMPageFormatGetPrinterID(\_:\_:)

Obtains the identifier of the formatting printer for a page format object.

macOS 10.5+

``` source
func PMPageFormatGetPrinterID(
    _ pageFormat: PMPageFormat,
    _ printerID: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object whose printer identifier you want to obtain.

`printerID`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string that contains the identifier of the formatting printer for the specified page format object. If the page format object does not have that information, the variable is set to `NULL`. You should not release the string without first retaining it.

## Return Value

A result code. See Result Codes.

## Discussion

Page format objects can be created a number of different ways and some of them do not require a specific printer. If the printer ID is known, the printer is displayed in the Page Setup dialog’s Format for pop-up menu. If the printer ID is not known, the default formatting printer is the generic Any Printer. The printing system provides default page and paper sizes for the generic printer.

## See Also

### Accessing Data in Page Format Objects

func PMGetPageFormatExtendedData(PMPageFormat, OSType, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?) -> OSStatus

Obtains extended page format data previously stored by your application.

func PMSetPageFormatExtendedData(PMPageFormat, OSType, UInt32, UnsafeMutableRawPointer) -> OSStatus

Stores your application-specific data in a page format object.

func PMGetPageFormatPaper(PMPageFormat, UnsafeMutablePointer&lt;PMPaper?>) -> OSStatus

Obtains the paper associated with a page format object.

func PMGetOrientation(PMPageFormat, UnsafeMutablePointer&lt;PMOrientation>) -> OSStatus

Obtains the current setting for page orientation.

func PMSetOrientation(PMPageFormat, PMOrientation, Bool) -> OSStatus

Sets the page orientation for printing.

func PMGetScale(PMPageFormat, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the scaling factor currently applied to the page and paper rectangles.

func PMSetScale(PMPageFormat, Double) -> OSStatus

Sets the scaling factor for the page and paper rectangles.

func PMGetAdjustedPageRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the imageable area or page rectangle, taking into account orientation, application drawing resolution, and scaling settings.

func PMGetAdjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the rectangle defining the paper size, taking into account orientation, application drawing resolution, and scaling settings.

func PMGetUnadjustedPageRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the imageable area or page rectangle, unaffected by orientation, resolution, or scaling.

func PMGetUnadjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the paper rectangle, unaffected by rotation, resolution, or scaling.

