

- Application Services
- Core Printing
-  PMSessionSetCurrentPMPrinter(\_:\_:) 

Function

# PMSessionSetCurrentPMPrinter(\_:\_:)

Changes the current printer for a printing session.

macOS 10.3+

``` source
func PMSessionSetCurrentPMPrinter(
    _ session: PMPrintSession,
    _ printer: PMPrinter
) -> OSStatus
```

## Parameters 

`session`  

The printing session whose printer you want to change.

`printer`  

The new printer for the printing session.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

## See Also

### Accessing Data in Printing Session Objects

func PMSessionGetDataFromSession(PMPrintSession, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>) -> OSStatus

Obtains application-specific data previously stored in a printing session object.

func PMSessionSetDataInSession(PMPrintSession, CFString, CFTypeRef) -> OSStatus

Stores your application-specific data in a printing session object.

func PMSessionGetCurrentPrinter(PMPrintSession, UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Obtains the current printer associated with a printing session.

func PMSessionGetCGGraphicsContext(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CGContext>?>) -> OSStatus

Obtains the Quartz graphics context for the current page in a printing session.

func PMSessionError(PMPrintSession) -> OSStatus

Obtains the result code for any error returned by the printing session.

func PMSessionSetError(PMPrintSession, OSStatus) -> OSStatus

Sets the value of the current result code for the specified printing session.

