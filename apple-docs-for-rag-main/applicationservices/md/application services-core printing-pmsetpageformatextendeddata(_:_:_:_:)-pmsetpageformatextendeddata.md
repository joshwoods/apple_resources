

- Application Services
- Core Printing
-  PMSetPageFormatExtendedData(\_:\_:\_:\_:) 

Function

# PMSetPageFormatExtendedData(\_:\_:\_:\_:)

Stores your application-specific data in a page format object.

macOS 10.0+

``` source
func PMSetPageFormatExtendedData(
    _ pageFormat: PMPageFormat,
    _ dataID: OSType,
    _ size: UInt32,
    _ extendedData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object in which to store your extended data.

`dataID`  

A 4-character code that identifies your data. This is typically your application’s creator code. If your creator code is outside the ASCII 7-bit character range 0x20–0x7F, you need to use a different 4-character code.

`size`  

The size, in bytes, of the data to be stored in the page format object.

`extendedData`  

A pointer to the application-specific data you want to store in the page format object.

## Return Value

A result code. See Result Codes.

## Discussion

You can retrieve the data you store with the function `PMSetPageFormatExtendedData` by calling the function `PMGetPageFormatExtendedData`.

## See Also

### Accessing Data in Page Format Objects

func PMGetPageFormatExtendedData(PMPageFormat, OSType, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?) -> OSStatus

Obtains extended page format data previously stored by your application.

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

func PMGetUnadjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the paper rectangle, unaffected by rotation, resolution, or scaling.

