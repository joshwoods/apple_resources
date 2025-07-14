

- Application Services
- Core Printing
-  PMPaperGetPPDPaperName(\_:\_:) 

Function

# PMPaperGetPPDPaperName(\_:\_:)

Obtains the PPD paper name for a given paper.

macOS 10.5+

``` source
func PMPaperGetPPDPaperName(
    _ paper: PMPaper,
    _ paperName: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose PPD paper name you want to obtain.

`paperName`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string that contains the PPD paper name for the specified paper. If an error occurs, the variable is set to `NULL`. You should not release the string without first retaining it.

## Return Value

A result code. See Result Codes.

## Discussion

The macOS printing system uses a PostScript Printer Description (PPD) file to describe a given printer and print queue for that printer. The PPD paper name is the name that uniquely identifies a given paper for the printer to which the paper corresponds. To obtain a list of papers for a given printer, use the function PMPrinterGetPaperList(_:_:).

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

func PMPaperGetPrinterID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the printer ID of the printer to which a given paper corresponds.

