

- Application Services
- Core Printing
-  PMPrinterGetIndexedPrinterResolution(\_:\_:\_:) 

Function

# PMPrinterGetIndexedPrinterResolution(\_:\_:\_:)

Obtains a resolution setting based on an index into the range of settings supported by the specified printer.

macOS 10.0+

``` source
func PMPrinterGetIndexedPrinterResolution(
    _ printer: PMPrinter,
    _ index: UInt32,
    _ resolutionP: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`printer`  

The printer whose resolution you want to obtain.

`index`  

An index into the range of resolution settings supported by the specified printer. Index values begin at 1.

`res`  

A pointer to your PMResolution data structure. On return, the structure contains the printer resolution setting associated with the index value.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. Before you call this function, you must call the function PMPrinterGetPrinterResolutionCount(_:_:) to obtain the number of resolution settings supported by the specified printer.

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

