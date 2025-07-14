

- Application Services
- Core Printing
-  PMServerCreatePrinterList(\_:\_:) 

Function

# PMServerCreatePrinterList(\_:\_:)

Creates a list of printers available to a print server.

macOS 10.2+

``` source
func PMServerCreatePrinterList(
    _ server: PMServer?,
    _ printerList: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`server`  

The print server whose printers you want to obtain. To specify the local print server, pass the constant `kPMServerLocal`. Currently, you may specify only the local print server.

`printerList`  

A pointer to your CFArray variable. On return, the variable refers to a Core Foundation array containing the printers available to the specified print server. Each element in the array is a `PMPrinter` object. You are responsible for releasing the array.

## Return Value

A result code. See Result Codes.

## See Also

### Creating Printer Objects

func PMServerLaunchPrinterBrowser(PMServer?, CFDictionary?) -> OSStatus

Launches the printer browser to browse the printers available for a print server.

func PMSessionCreatePrinterList(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>, UnsafeMutablePointer&lt;CFIndex>?, UnsafeMutablePointer&lt;PMPrinter?>?) -> OSStatus

Creates a list of printers available in the specified printing session.

func PMPrinterCreateFromPrinterID(CFString) -> PMPrinter?

Creates a printer object from a print queue identifier.

func PMCreateGenericPrinter(UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Creates a generic printer object.

