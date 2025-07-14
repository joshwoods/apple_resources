

- Application Services
- Core Printing
-  PMSessionCopyOutputFormatList(\_:\_:\_:) 

Function

# PMSessionCopyOutputFormatList(\_:\_:\_:)

Obtains an array of destination formats supported by the current print destination.

macOS 10.1+

``` source
func PMSessionCopyOutputFormatList(
    _ printSession: PMPrintSession,
    _ destType: PMDestinationType,
    _ documentFormatP: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session that provides a context for the print job. The printer associated with this session is queried for the MIME types it supports.

`destType`  

A destination type that specifies the destination for which you want to obtain valid destination formats. See PMDestinationType for a list of the possible destination types a print job can have.

`documentFormatP`  

A pointer to your CFArray variable. On return, the variable refers to a Core Foundation array that contains a list of destination formats that can be generated for the current print destination. See Document Format Strings for a list of some of the output formats that can be returned.

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

func PMSessionCopyDestinationFormat(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the destination format for a print job.

func PMSessionCopyDestinationLocation(PMPrintSession, PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains a destination location for a print job.

