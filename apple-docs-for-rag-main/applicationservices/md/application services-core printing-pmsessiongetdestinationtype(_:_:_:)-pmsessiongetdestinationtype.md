

- Application Services
- Core Printing
-  PMSessionGetDestinationType(\_:\_:\_:) 

Function

# PMSessionGetDestinationType(\_:\_:\_:)

Obtains the output destination for a print job.

macOS 10.1+

``` source
func PMSessionGetDestinationType(
    _ printSession: PMPrintSession,
    _ printSettings: PMPrintSettings,
    _ destTypeP: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session that provides a context for the print job. This must be the same printing session used for the Print dialog. The printing session contains the preview setting, which can override the destination type in the print settings.

`printSettings`  

The print settings for the print job whose destination you want to obtain.

`destTypeP`  

A pointer to your `PMDestinationType` variable. On return, the variable contains the destination type for the specified print job. Possible values include:

- `kPMDestinationPrinter` (output to a printer)

- `kPMDestinationFile` (output to a file)

- `kPMDestinationFax` (output to a fax)

- `kPMDestinationPreview` (output to print preview)

- `kPMDestinationProcessPDF` (output to a PDF workflow option)

See PMDestinationType for a complete description of the destination type constants.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

All of the destination types are stored in the print settings object except for `kPMDestinationPreview`, which is stored in the printing session object. If the destination type is set as preview, the preview setting overrides the destination set in the print settings object.

## See Also

### Accessing the Print Job Destination

func PMSessionSetDestination(PMPrintSession, PMPrintSettings, PMDestinationType, CFString?, CFURL?) -> OSStatus

Sets the destination location, format, and type for a print job.

func PMSessionCopyDestinationFormat(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the destination format for a print job.

func PMSessionCopyDestinationLocation(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains a destination location for a print job.

func PMSessionCopyOutputFormatList(PMPrintSession, PMDestinationType, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains an array of destination formats supported by the current print destination.

