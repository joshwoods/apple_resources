

- Application Services
- Core Printing
-  PMGetUnadjustedPageRect(\_:\_:) 

Function

# PMGetUnadjustedPageRect(\_:\_:)

Obtains the imageable area or page rectangle, unaffected by orientation, resolution, or scaling.

macOS 10.0+

``` source
func PMGetUnadjustedPageRect(
    _ pageFormat: PMPageFormat,
    _ pageRect: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object whose unadjusted page rectangle you want to obtain.

`pageRect`  

A pointer to your PMRect data structure. On return, the structure contains the size of the page rectangle, in points. The page rectangle is the area of the page to which an application can draw. The coordinates for the upper-left corner of the page rectangle are (0,0). See Supporting Printing in Your Carbon Application for more information on page and paper rectangles.

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

func PMGetScale(PMPageFormat, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the scaling factor currently applied to the page and paper rectangles.

func PMSetScale(PMPageFormat, Double) -> OSStatus

Sets the scaling factor for the page and paper rectangles.

func PMGetAdjustedPageRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the imageable area or page rectangle, taking into account orientation, application drawing resolution, and scaling settings.

func PMGetAdjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the rectangle defining the paper size, taking into account orientation, application drawing resolution, and scaling settings.

func PMGetUnadjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the paper rectangle, unaffected by rotation, resolution, or scaling.

