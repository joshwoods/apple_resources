

- Application Services
- Core Printing
-  PMSessionSetDestination(\_:\_:\_:\_:\_:) 

Function

# PMSessionSetDestination(\_:\_:\_:\_:\_:)

Sets the destination location, format, and type for a print job.

macOS 10.1+

``` source
func PMSessionSetDestination(
    _ printSession: PMPrintSession,
    _ printSettings: PMPrintSettings,
    _ destType: PMDestinationType,
    _ destFormat: CFString?,
    _ destLocation: CFURL?
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session that provides a context for the print job.

`printSettings`  

The print settings for the print job whose destination you want to set.

`destType`  

The destination type for the print job associated with the specified printing session and print settings. Possible values include:

- `kPMDestinationPrinter` (output to a printer)

- `kPMDestinationFile` (output to a file)

- `kPMDestinationFax` (output to a fax)

- `kPMDestinationPreview` (output to print preview)

- `kPMDestinationProcessPDF` (output to a PDF workflow option)

See PMDestinationType for a complete description of destination types you can specify.

`destFormat`  

The MIME type to be generated for the specified destination type. Pass `NULL` if you want to use the default format for the specified destination type. To obtain a list of valid formats for a given destination type, use the function PMSessionCopyOutputFormatList(_:_:_:).

`destLocation`  

A reference to a Core Foundation URL that specifies a destination location. You can provide this if the destination type supports a destination location. Otherwise, pass `NULL`. For example, if the destination type is a file (`kPMDestinationFile`) you can supply a file system URL to specify where the file resides.

## Return Value

A result code. See Result Codes.

## Discussion

You can use the function `PMSessionSetDestination` when you want to send print output to a file without requiring user interaction. You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

## See Also

### Accessing the Print Job Destination

func PMSessionGetDestinationType(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;PMDestinationType>) -> OSStatus

Obtains the output destination for a print job.

func PMSessionCopyDestinationFormat(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the destination format for a print job.

func PMSessionCopyDestinationLocation(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains a destination location for a print job.

func PMSessionCopyOutputFormatList(PMPrintSession, PMDestinationType, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains an array of destination formats supported by the current print destination.

