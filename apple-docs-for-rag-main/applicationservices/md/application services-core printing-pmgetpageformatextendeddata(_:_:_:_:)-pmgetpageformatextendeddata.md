

- Application Services
- Core Printing
-  PMGetPageFormatExtendedData(\_:\_:\_:\_:) 

Function

# PMGetPageFormatExtendedData(\_:\_:\_:\_:)

Obtains extended page format data previously stored by your application.

macOS 10.0+

``` source
func PMGetPageFormatExtendedData(
    _ pageFormat: PMPageFormat,
    _ dataID: OSType,
    _ size: UnsafeMutablePointer?,
    _ extendedData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object that contains your extended data.

`dataID`  

A 4-character code that identifies your data. This is typically your application’s creator code. If your creator code is outside the ASCII 7-bit character range 0x20–0x7F, you need to use a different 4-character code.

`size`  

A pointer to a value that specifies the size of the buffer you have allocated for the extended page format data. On return, this variable contains the number of bytes read into the buffer or the size of the extended data. You can pass the constant `kPMDontWantSize` if you do not need this information. (See Data Not Wanted Constants for more information.)

`extendedData`  

A pointer to a buffer to receive the extended data. Pass the constant `kPMDontWantData` if you do not want to read the data. (See Data Not Wanted Constants for more information.)

## Return Value

A result code. See Result Codes.

## Discussion

Your application typically needs to call the function `PMGetPageFormatExtendedData` two times in order to retrieve the extended page format data. The first time, pass the constant `kPMDontWantData` in the parameter `extendedData` to obtain the buffer size required for the extended data. Then allocate the buffer and call the function a second time to read the extended data into your buffer.

If you write a printing dialog extension for your application that stores data in the page format object, you use the function `PMGetPageFormatExtendedData` to retrieve the data associated with it.

## See Also

### Accessing Data in Page Format Objects

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

func PMGetUnadjustedPaperRect(PMPageFormat, UnsafeMutablePointer&lt;PMRect>) -> OSStatus

Obtains the paper rectangle, unaffected by rotation, resolution, or scaling.

