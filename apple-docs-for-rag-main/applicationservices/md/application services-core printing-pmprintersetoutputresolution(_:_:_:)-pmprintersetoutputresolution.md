

- Application Services
- Core Printing
-  PMPrinterSetOutputResolution(\_:\_:\_:) 

Function

# PMPrinterSetOutputResolution(\_:\_:\_:)

Sets the print settings to reflect the specified printer hardware output resolution.

macOS 10.5+

``` source
func PMPrinterSetOutputResolution(
    _ printer: PMPrinter,
    _ printSettings: PMPrintSettings,
    _ resolutionP: UnsafePointer
) -> OSStatus
```

## Parameters 

`printer`  

The printer whose output resolution you want to change.

`printSettings`  

The print settings object used for the print job.

`resolutionP`  

A pointer to a PMResolution structure that specifies the desired resolution in pixels per inch.

## Return Value

A result code. See Result Codes.

## Discussion

Some printers allow programmatic control of their hardware output resolution on a print job basis. The hardware resolution is determined by the combination of printer and print settings used for the print job. This function configures the print settings to the closest resolution setting that can be used for the destination print job. Note that not all printers allow control of their resolution setting.

This function is rarely used. Most applications do not set the output resolution but instead use the setting supplied by the user in the Print dialog.

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

