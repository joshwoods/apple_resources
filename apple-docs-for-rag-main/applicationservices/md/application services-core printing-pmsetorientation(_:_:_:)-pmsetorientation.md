

- Application Services
- Core Printing
-  PMSetOrientation(\_:\_:\_:) 

Function

# PMSetOrientation(\_:\_:\_:)

Sets the page orientation for printing.

macOS 10.0+

``` source
func PMSetOrientation(
    _ pageFormat: PMPageFormat,
    _ orientation: PMOrientation,
    _ lock: Bool
) -> OSStatus
```

## Parameters 

`pageFormat`  

The page format object whose page orientation you want to set.

`orientation`  

A constant specifying the desired page orientation. Supported values are:

- `kPMPortrait`

- `kPMLandscape`

- `kPMReversePortrait` (macOS 10.5 and later)

- `kPMReverseLandscape`

See PMOrientation for a full description of the values you can use to specify page orientation.

`lock`  

The lock state of the setting. You should pass `kPMUnlocked`. Locking is not supported at this time.

## Return Value

A result code. See Result Codes.

## Discussion

In OS X v10.4 and earlier, if you want to set the page orientation you need to call this function before initiating the print job (for example, by calling `PMSessionBeginCGDocument`). The page orientation you set applies to the entire print job. In macOS 10.5 and later, you can use this function to change the orientation of an individual page in a print job by passing the updated page format to `PMSessionBeginPage` or `PMSessionBeginPageNoDialog`.

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

