

- Application Services
- Core Printing
-  PMGetScale(\_:\_:) 

Function

# PMGetScale(\_:\_:)

Obtains the scaling factor currently applied to the page and paper rectangles.

macOS 10.0+

``` source
func PMGetScale(
    _ pageFormat: PMPageFormat,
    _ scale: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object whose scaling factor you want to obtain.

`scale`  

A pointer to your double-precision variable. On return, the variable contains the scaling factor expressed as a percentage. For example, a value of 100.0 means 100 percent (that is, no scaling); a value of 50.0 means 50 percent scaling.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing Data in Page Format Objects

func PMGetPageFormatExtendedData(PMPageFormat, OSType, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?) -> OSStatus

Obtains extended page format data previously stored by your application.

func PMSetPageFormatExtendedData(PMPageFormat, OSType, UInt32, UnsafeMutableRawPointer) -> OSStatus

Stores your application-specific data in a page format object.

func PMGetPageFormatPaper(PMPageFormat, UnsafeMutablePointer&lt;PMPaper?>) -> OSStatus

Obtains the paper associated with a page format object.

func PMPageFormatGetPrinterID(PMPageFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the identifier of the formatting printer for a page format object.

func PMGetOrientation(PMPageFormat, UnsafeMutablePointer&lt;PMOrientation>) -> OSStatus

Obtains the current setting for page orientation.

func PMSetOrientation(PMPageFormat, PMOrientation, Bool) -> OSStatus

Sets the page orientation for printing.

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

