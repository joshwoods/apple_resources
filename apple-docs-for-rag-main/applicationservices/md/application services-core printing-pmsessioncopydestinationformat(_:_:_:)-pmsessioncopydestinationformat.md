

- Application Services
- Core Printing
-  PMSessionCopyDestinationFormat(\_:\_:\_:) 

Function

# PMSessionCopyDestinationFormat(\_:\_:\_:)

Obtains the destination format for a print job.

macOS 10.1+

``` source
func PMSessionCopyDestinationFormat(
    _ printSession: PMPrintSession,
    _ printSettings: PMPrintSettings,
    _ destFormatP: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session that provides a context for the print job.

`printSettings`  

The print settings object for the print job whose destination format you want to obtain.

`destFormatP`  

A pointer to your CFString variable. On return, the variable refers to a Core Foundation string that contains the destination format for the print job. You are responsible for releasing the string. Currently, there are two possible values: `kPMDocumentFormatPDF` or `kPMDocumentFormatPostScript`.

If an error occurs, the variable is set to `NULL`. If the function executes without error and the variable is set to `NULL`, the print job is set to use the default destination format.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

## See Also

### Accessing the Print Job Destination

func PMSessionSetDestination(PMPrintSession, PMPrintSettings, PMDestinationType, CFString?, CFURL?) -> OSStatus

Sets the destination location, format, and type for a print job.

func PMSessionGetDestinationType(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;PMDestinationType>) -> OSStatus

Obtains the output destination for a print job.

func PMSessionCopyDestinationLocation(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains a destination location for a print job.

func PMSessionCopyOutputFormatList(PMPrintSession, PMDestinationType, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains an array of destination formats supported by the current print destination.

