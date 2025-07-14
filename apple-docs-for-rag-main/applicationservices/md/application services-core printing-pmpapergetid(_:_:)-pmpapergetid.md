

- Application Services
- Core Printing
-  PMPaperGetID(\_:\_:) 

Function

# PMPaperGetID(\_:\_:)

Obtains the identifier of a paper object.

macOS 10.3+

``` source
func PMPaperGetID(
    _ paper: PMPaper,
    _ paperID: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose identifier you want to obtain.

`paperID`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string containing the unique identifier for this paper. You should not release the string without first retaining it.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing Data in Paper Objects

func PMPaperGetWidth(PMPaper, UnsafeMutablePointer&lt;Double>) -> OSStatus

Obtains the width of the sheet of paper represented by a paper object.

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

