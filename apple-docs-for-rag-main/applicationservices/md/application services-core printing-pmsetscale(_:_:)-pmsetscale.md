

- Application Services
- Core Printing
-  PMSetScale(\_:\_:) 

Function

# PMSetScale(\_:\_:)

Sets the scaling factor for the page and paper rectangles.

macOS 10.0+

``` source
func PMSetScale(
    _ pageFormat: PMPageFormat,
    _ scale: Double
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object whose scaling factor you want to set.

`scale`  

The desired scaling factor expressed as a percentage. For example, for 50 percent scaling, pass a value of 50.0; for no scaling, pass 100.0.

## Return Value

A result code. See Result Codes.

## Discussion

You can call the function `PMSetScale` to change the scaling factor that appears when your application invokes the Page Setup dialog.

If you call `PMSetScale` after calling `PMSessionPageSetupDialog`, make sure you call PMSessionValidatePageFormat(_:_:_:) before you call `PMSessionBeginCGDocument` or PMSessionBeginDocument.

If you call this function after initiating a print job, the change is ignored for the current job.

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

func PMGetAdjustedPageRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the imageable area or page rectangle, taking into account orientation, application drawing resolution, and scaling settings.

func PMGetAdjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the rectangle defining the paper size, taking into account orientation, application drawing resolution, and scaling settings.

func PMGetUnadjustedPageRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the imageable area or page rectangle, unaffected by orientation, resolution, or scaling.

func PMGetUnadjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the paper rectangle, unaffected by rotation, resolution, or scaling.

