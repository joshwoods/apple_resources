

- Application Services
- Core Printing
-  PMPrinterCreateFromPrinterID(\_:) 

Function

# PMPrinterCreateFromPrinterID(\_:)

Creates a printer object from a print queue identifier.

macOS 10.4+

``` source
func PMPrinterCreateFromPrinterID(_ printerID: CFString) -> PMPrinter?
```

## Parameters 

`printerID`  

The unique identifier of a print queue.

## Return Value

A new printer object, or `NULL` if no print queue is available with the specified identifier. You are responsible for releasing the printer object with the function PMRelease(_:).

## Discussion

This function is typically used to re-create a printer object using the print queue ID obtained by a call to `PMPrinterGetID` at an earlier time. If the print queue is deleted after obtaining the ID, this function returns `NULL` for that ID.

## See Also

### Creating Printer Objects

func PMServerLaunchPrinterBrowser(PMServer?, CFDictionary?) -> OSStatus

Launches the printer browser to browse the printers available for a print server.

func PMServerCreatePrinterList(PMServer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Creates a list of printers available to a print server.

func PMSessionCreatePrinterList(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>, UnsafeMutablePointer&lt;CFIndex>?, UnsafeMutablePointer&lt;PMPrinter?>?) -> OSStatus

Creates a list of printers available in the specified printing session.

func PMCreateGenericPrinter(UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Creates a generic printer object.

### Related Documentation

func PMPrinterGetID(PMPrinter) -> Unmanaged&lt;CFString>?

Returns the unique identifier of a printer.

