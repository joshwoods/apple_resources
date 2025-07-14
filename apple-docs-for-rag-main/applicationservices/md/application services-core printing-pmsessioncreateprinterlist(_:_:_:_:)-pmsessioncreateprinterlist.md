

- Application Services
- Core Printing
-  PMSessionCreatePrinterList(\_:\_:\_:\_:) 

Function

# PMSessionCreatePrinterList(\_:\_:\_:\_:)

Creates a list of printers available in the specified printing session.

macOS 10.1+

``` source
func PMSessionCreatePrinterList(
    _ printSession: PMPrintSession,
    _ printerList: UnsafeMutablePointer?>,
    _ currentIndex: UnsafeMutablePointer?,
    _ currentPrinter: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session whose printer list you want to obtain.

`printerList`  

A pointer to your CFArray variable. On return, the variable refers to a Core Foundation array containing a list of printers available in the specified printing session. Each element in the array is a Core Foundation string that contains a printer’s name as shown in the user interface. You are responsible for releasing the array.

`currentIndex`  

A pointer to your CFIndex variable. On return, the variable contains a value specifying where the current printer is in the printer list.

`currentPrinter`  

A pointer to your PMPrinter variable. On return, the variable refers to a printer object that represents the current printer. You should not release the printer object without first retaining it. If the printer is the generic printer, the variable is set to `NULL`.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

You can call the function `PMSessionCreatePrinterList` to obtain a valid printer name to pass to the function `PMSessionSetCurrentPrinter`.

### Special Considerations

In macOS 10.2 and later, Apple recommends using the function PMServerCreatePrinterList(_:_:) instead. `PMServerCreatePrinterList` doesn’t require a `PMSession` object; it can be called at any time. It also works directly with `PMPrinter` objects.

## See Also

### Creating Printer Objects

func PMServerLaunchPrinterBrowser(PMServer?, CFDictionary?) -> OSStatus

Launches the printer browser to browse the printers available for a print server.

func PMServerCreatePrinterList(PMServer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Creates a list of printers available to a print server.

func PMPrinterCreateFromPrinterID(CFString) -> PMPrinter?

Creates a printer object from a print queue identifier.

func PMCreateGenericPrinter(UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Creates a generic printer object.

