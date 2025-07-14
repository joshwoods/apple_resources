

- Application Services
- Core Printing
-  PMSessionCopyDestinationLocation(\_:\_:\_:) 

Function

# PMSessionCopyDestinationLocation(\_:\_:\_:)

Obtains a destination location for a print job.

macOS 10.1+

``` source
func PMSessionCopyDestinationLocation(
    _ printSession: PMPrintSession,
    _ printSettings: PMPrintSettings,
    _ destLocationP: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session that provides a context for the print job.

`printSettings`  

The print settings for the print job whose destination location you want to obtain.

`destLocationP`  

A pointer to your CFURL variable. On return, the variable refers to a Core Foundation URL that specifies the destination location of the print job. You are responsible for releasing the URL. If `NULL` is returned and the function executes without error (result code is `noErr`), the print job uses the default destination location for the current destination type. If an error occurs, the variable is set to `NULL`.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

Some destination types define a specific kind of destination location for a print job. For example, the destination type `kPMDestinationFile` uses a file system URL to specify where a new file should be created for the print job’s output.

## See Also

### Accessing the Print Job Destination

func PMSessionSetDestination(PMPrintSession, PMPrintSettings, PMDestinationType, CFString?, CFURL?) -> OSStatus

Sets the destination location, format, and type for a print job.

func PMSessionGetDestinationType(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;PMDestinationType>) -> OSStatus

Obtains the output destination for a print job.

func PMSessionCopyDestinationFormat(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the destination format for a print job.

func PMSessionCopyOutputFormatList(PMPrintSession, PMDestinationType, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains an array of destination formats supported by the current print destination.

