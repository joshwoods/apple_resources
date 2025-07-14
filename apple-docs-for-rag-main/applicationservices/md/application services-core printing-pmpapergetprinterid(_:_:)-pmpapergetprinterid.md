

- Application Services
- Core Printing
-  PMPaperGetPrinterID(\_:\_:) 

Function

# PMPaperGetPrinterID(\_:\_:)

Obtains the printer ID of the printer to which a given paper corresponds.

macOS 10.5+

``` source
func PMPaperGetPrinterID(
    _ paper: PMPaper,
    _ printerID: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose printer ID you want to obtain.

`printerID`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string that contains the printer ID for the specified paper. If an error occurs, the variable is set to `NULL`. You should not release the string without first retaining it.

## Return Value

A result code. See Result Codes.

## Discussion

Not all papers have a printer ID associated with them. If the printer ID is known, the printer is displayed in the Page Setup dialog’s Format for pop-up menu. If the printer ID is not known, the default formatting printer is the generic Any Printer. The printing system provides default paper sizes for the generic printer.

## See Also

### Accessing Data in Paper Objects

func PMPaperGetID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the identifier of a paper object.

func PMPaperGetWidth(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the width of the sheet of paper represented by a paper object.

func PMPaperGetHeight(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the height of the sheet of paper represented by a paper object.

func PMPaperGetMargins(PMPaper, UnsafeMutablePointer&lt;PMPaperMargins>) -> OSStatus

Obtains the margins describing the unprintable area of the sheet represented by a paper object.

func PMPaperCreateLocalizedName(PMPaper, PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the localized name for a given paper.

func PMPaperGetPPDPaperName(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the PPD paper name for a given paper.

