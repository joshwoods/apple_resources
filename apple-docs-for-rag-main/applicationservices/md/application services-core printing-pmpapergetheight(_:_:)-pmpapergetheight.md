

- Application Services
- Core Printing
-  PMPaperGetHeight(\_:\_:) 

Function

# PMPaperGetHeight(\_:\_:)

Obtains the height of the sheet of paper represented by a paper object.

macOS 10.3+

``` source
func PMPaperGetHeight(
    _ paper: PMPaper,
    _ paperHeight: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose height you want to obtain.

`paperHeight`  

A pointer to your double-precision variable. On return, the variable contains the height of the specified paper, in points.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing Data in Paper Objects

func PMPaperGetID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the identifier of a paper object.

func PMPaperGetWidth(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the width of the sheet of paper represented by a paper object.

func PMPaperGetMargins(PMPaper, UnsafeMutablePointer&lt;PMPaperMargins>) -> OSStatus

Obtains the margins describing the unprintable area of the sheet represented by a paper object.

func PMPaperCreateLocalizedName(PMPaper, PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the localized name for a given paper.

func PMPaperGetPrinterID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the printer ID of the printer to which a given paper corresponds.

func PMPaperGetPPDPaperName(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the PPD paper name for a given paper.

