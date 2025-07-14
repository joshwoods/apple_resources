

- Application Services
- Core Printing
-  PMPrinterGetOutputResolution(\_:\_:\_:) 

Function

# PMPrinterGetOutputResolution(\_:\_:\_:)

Obtains the printer hardware output resolution for the specified print settings.

macOS 10.5+

``` source
func PMPrinterGetOutputResolution(
    _ printer: PMPrinter,
    _ printSettings: PMPrintSettings,
    _ resolutionP: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`printer`  

The printer whose output resolution you want to obtain.

`printSettings`  

The print settings you want to use.

`resolutionP`  

A pointer to your PMResolution structure. On return, the structure contains the output resolution of the specified printer in pixels per inch.

## Return Value

A result code. If the resolution cannot be reliably determined, this function returns an error.

## Discussion

Some printers allow programmatic control of their hardware output resolution on a print job basis. The hardware resolution is determined by the combination of printer and print settings used for the print job. This function returns the best guess as to what printer resolution setting will be used for the destination print job.

Most applications do not need to use this function because they draw the same content regardless of the destination device. For those few applications that do adjust their drawing based on the output device, they should only do so when the print job destination is `kPMDestinationPrinter` or `kPMDestinationFax`. You can use the function `PMSessionGetDestinationType` to determine the destination for a print job.

This function should be used after displaying the Print dialog to the user so that it correctly reflects changes in print settings performed prior to printing.

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

func PMPrinterIsRemote(PMPrinter, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether a printer is hosted by a remote print server.

