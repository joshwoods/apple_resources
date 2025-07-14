

- Application Services
- Core Printing
-  PMPaperCreateLocalizedName(\_:\_:\_:) 

Function

# PMPaperCreateLocalizedName(\_:\_:\_:)

Obtains the localized name for a given paper.

macOS 10.5+

``` source
func PMPaperCreateLocalizedName(
    _ paper: PMPaper,
    _ printer: PMPrinter,
    _ paperName: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`paper`  

The paper whose localized name you want to obtain.

`printer`  

The printer for which the localization should be performed.

`paperName`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string that contains the localized name of the paper. This name is appropriate to display in the user interface. If an error occurs, the variable is set to `NULL`. You are responsible for releasing the string.

## Return Value

A result code. See Result Codes.

## Discussion

Not all printers have the same way of referring to a given paper. Generally, if you want to obtain the name of a paper, you want to localize the paper name for a particular printer. For example, if you were displaying a list of papers for a given printer, you would want the paper names to be localized for that printer.

### Special Considerations

In macOS 10.5 and later, Apple recommends using this function instead of PMPaperGetName.

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

func PMPaperGetPrinterID(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the printer ID of the printer to which a given paper corresponds.

func PMPaperGetPPDPaperName(PMPaper, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the PPD paper name for a given paper.

