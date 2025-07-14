

- Application Services
- Core Printing
-  PMPaperGetWidth(\_:\_:) 

Function

# PMPaperGetWidth(\_:\_:)

Obtains the width of the sheet of paper represented by a paper object.

macOS 10.3+

``` source
func PMPaperGetWidth(
    _ paper: PMPaper,
    _ paperWidth: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose width you want to obtain.

`paperWidth`  

A pointer to your double-precision variable. On return, the variable contains the width of the specified paper, in points.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing Data in Paper Objects

func PMPaperGetID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the identifier of a paper object.

func PMPaperGetHeight(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the height of the sheet of paper represented by a paper object.

func PMPaperGetMargins(PMPaper, UnsafeMutablePointer&lt;PMPaperMargins>) -> OSStatus

Obtains the margins describing the unprintable area of the sheet represented by a paper object.

func PMPaperCreateLocalizedName(PMPaper, PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the localized name for a given paper.

func PMPaperGetPrinterID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the printer ID of the printer to which a given paper corresponds.

func PMPaperGetPPDPaperName(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the PPD paper name for a given paper.

