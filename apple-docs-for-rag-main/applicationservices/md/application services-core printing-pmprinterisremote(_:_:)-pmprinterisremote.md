

- Application Services
- Core Printing
-  PMPrinterIsRemote(\_:\_:) 

Function

# PMPrinterIsRemote(\_:\_:)

Indicates whether a printer is hosted by a remote print server.

macOS 10.3+

``` source
func PMPrinterIsRemote(
    _ printer: PMPrinter,
    _ isRemoteP: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`printer`  

The printer you’re querying to determine whether it is hosted by a remote print server.

`isRemoteP`  

A pointer to your Boolean variable. On return, `true` indicates that the printer is hosted by a remote print server; otherwise, `false`.

## Return Value

A result code. See Result Codes.

## Discussion

If this function returns `true`, the printer is hosted by a remote print server and the printer can be considered a shared printer.

In macOS, the typical way that users create a print queue for a shared printer is by browsing. Print queues for shared printers that are created by browsing are marked as remote queues, and `PMPrinterIsRemote` returns `true` for such printers. However, expert users can create a local queue for a remote printer manually, and such a printer does not appear to be remote printer.

Whether a printer is remote is derived from the CUPS printer-type attribute for the print queue.

## See Also

### Accessing Information About a Printer

func PMPrinterCopyDescriptionURL(PMPrinter, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains the URL of the description file for a given printer.

func PMPrinterCopyDeviceURI(PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains the device URI of a given printer.

func PMPrinterCopyHostName(PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the name of the server hosting the print queue for a given printer.

func PMPrinterCopyPresets(PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains a list of print settings presets for a printer.

func PMPrinterGetCommInfo(PMPrinter, UnsafeMutablePointer&lt;DarwinBoolean>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Obtains information about the communication channel for a printer.

func PMPrinterGetDriverCreator(PMPrinter, UnsafeMutablePointer&lt;OSType>) -> OSStatus

Obtains the creator of the driver associated with the specified printer.

func PMPrinterGetID(PMPrinter) -> Unmanaged&lt;CFString>?

Returns the unique identifier of a printer.

func PMPrinterGetLocation(PMPrinter) -> Unmanaged&lt;CFString>?

Returns the location of a printer.

func PMPrinterGetMakeAndModelName(PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the manufacturer and model name of the specified printer.

func PMPrinterGetMimeTypes(PMPrinter, PMPrintSettings?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains a list of MIME content types supported by a printer using the specified print settings.

func PMPrinterGetName(PMPrinter) -> Unmanaged&lt;CFString>?

Returns the human-readable name of a printer.

func PMPrinterGetOutputResolution(PMPrinter, PMPrintSettings, UnsafeMutablePointer&lt;PMResolution>) -> OSStatus

Obtains the printer hardware output resolution for the specified print settings.

func PMPrinterSetOutputResolution(PMPrinter, PMPrintSettings, UnsafePointer&lt;PMResolution>) -> OSStatus

Sets the print settings to reflect the specified printer hardware output resolution.

func PMPrinterGetPaperList(PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the list of papers available for a printer.

func PMPrinterGetPrinterResolutionCount(PMPrinter, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Obtains the number of resolution settings supported by the specified printer.

func PMPrinterGetIndexedPrinterResolution(PMPrinter, UInt32, UnsafeMutablePointer&lt;PMResolution>) -> OSStatus

Obtains a resolution setting based on an index into the range of settings supported by the specified printer.

func PMPrinterGetState(PMPrinter, UnsafeMutablePointer&lt;PMPrinterState>) -> OSStatus

Obtains the current state of the print queue for a printer.

func PMPrinterSetDefault(PMPrinter) -> OSStatus

Sets the default printer for the current user.

func PMPrinterIsDefault(PMPrinter) -> Bool

Returns a Boolean value indicating whether a printer is the default printer for the current user.

func PMPrinterIsFavorite(PMPrinter) -> Bool

Returns a Boolean value indicating whether a printer is in the user’s list of favorite printers.

func PMPrinterIsPostScriptCapable(PMPrinter) -> Bool

Returns a Boolean value indicating whether a printer is PostScript capable.

func PMPrinterIsPostScriptPrinter(PMPrinter, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether a printer is a PostScript printer.

