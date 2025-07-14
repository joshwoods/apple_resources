

- Application Services
- Core Printing
-  PMPaperGetMargins(\_:\_:) 

Function

# PMPaperGetMargins(\_:\_:)

Obtains the margins describing the unprintable area of the sheet represented by a paper object.

macOS 10.3+

``` source
func PMPaperGetMargins(
    _ paper: PMPaper,
    _ paperMargins: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose margins you want to obtain.

`paperMargins`  

A pointer to your PMPaperMargins structure. On return, the structure contains the unprintable margins of the specified paper, in points. The four values in the structure specify the top, left, bottom, and right imageable area margins of the paper.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing Data in Paper Objects

func PMPaperGetID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the identifier of a paper object.

func PMPaperGetWidth(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the width of the sheet of paper represented by a paper object.

func PMPaperGetHeight(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the height of the sheet of paper represented by a paper object.

func PMPaperCreateLocalizedName(PMPaper, PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the localized name for a given paper.

func PMPaperGetPrinterID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the printer ID of the printer to which a given paper corresponds.

func PMPaperGetPPDPaperName(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the PPD paper name for a given paper.

