

- Application Services
- Core Printing
-  PMServerLaunchPrinterBrowser(\_:\_:) 

Function

# PMServerLaunchPrinterBrowser(\_:\_:)

Launches the printer browser to browse the printers available for a print server.

macOS 10.5+

``` source
func PMServerLaunchPrinterBrowser(
    _ server: PMServer?,
    _ options: CFDictionary?
) -> OSStatus
```

## Parameters 

`server`  

The print server to browse. Pass `kPMServerLocal` to specify the local print server. Currently, you may specify only the local print server.

`options`  

This parameter is reserved for future use. At the present time, pass `NULL`. Passing `NULL` presents the printer browser in the default fashion.

## Return Value

A result code. See Result Codes. If you specify a server whose printers cannot be browsed, this function returns the error code `kPMInvalidParameter`.

## Discussion

This function displays the standard printer browser to allow the user to create a new print queue.

## See Also

### Creating Printer Objects

func PMServerCreatePrinterList(PMServer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Creates a list of printers available to a print server.

func PMSessionCreatePrinterList(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>, UnsafeMutablePointer&lt;CFIndex>?, UnsafeMutablePointer&lt;PMPrinter?>?) -> OSStatus

Creates a list of printers available in the specified printing session.

func PMPrinterCreateFromPrinterID(CFString) -> PMPrinter?

Creates a printer object from a print queue identifier.

func PMCreateGenericPrinter(UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Creates a generic printer object.

