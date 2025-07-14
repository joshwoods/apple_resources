

- Application Services
- Core Printing
-  PMCreateGenericPrinter(\_:) 

Function

# PMCreateGenericPrinter(\_:)

Creates a generic printer object.

macOS 10.5+

``` source
func PMCreateGenericPrinter(_ printer: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`printer`  

A pointer to your PMPrinter variable. On return, the variable refers to a new printer object that represents the generic formatting printer. You are responsible for releasing the printer object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## Discussion

This function provides a way to create a `PMPrinter` object that represents the generic formatting printer.

## See Also

### Creating Printer Objects

func PMServerLaunchPrinterBrowser(PMServer?, CFDictionary?) -> OSStatus

Launches the printer browser to browse the printers available for a print server.

func PMServerCreatePrinterList(PMServer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Creates a list of printers available to a print server.

func PMSessionCreatePrinterList(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>, UnsafeMutablePointer&lt;CFIndex>?, UnsafeMutablePointer&lt;PMPrinter?>?) -> OSStatus

Creates a list of printers available in the specified printing session.

func PMPrinterCreateFromPrinterID(CFString) -> PMPrinter?

Creates a printer object from a print queue identifier.

