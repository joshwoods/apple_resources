

- Application Services
- Core Printing
-  PMGetUnadjustedPaperRect(\_:\_:) 

Function

# PMGetUnadjustedPaperRect(\_:\_:)

Obtains the paper rectangle, unaffected by rotation, resolution, or scaling.

macOS 10.0+

``` source
func PMGetUnadjustedPaperRect(
    _ pageFormat: PMPageFormat,
    _ paperRect: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object whose unadjusted paper rectangle you want to obtain.

`paperRect`  

A pointer to your PMRect data structure. On return, the structure contains the physical size of the paper, in points. The coordinates of the upper-left corner of the paper rectangle are specified relative to the page rectangle. The coordinates of the upper-left corner of the page rectangle are always (0,0), which means the coordinates of the upper-left corner of the paper rectangle are always negative or (0,0). See Supporting Printing in Your Carbon Application for more information on page and paper rectangles.

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

func PMGetUnadjustedPageRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the imageable area or page rectangle, unaffected by orientation, resolution, or scaling.

