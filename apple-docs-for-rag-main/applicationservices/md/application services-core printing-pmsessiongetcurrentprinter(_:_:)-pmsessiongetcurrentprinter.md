

- Application Services
- Core Printing
-  PMSessionGetCurrentPrinter(\_:\_:) 

Function

# PMSessionGetCurrentPrinter(\_:\_:)

Obtains the current printer associated with a printing session.

macOS 10.0+

``` source
func PMSessionGetCurrentPrinter(
    _ printSession: PMPrintSession,
    _ currentPrinter: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session whose printer you want to obtain.

`currentPrinter`  

A pointer to your PMPrinter variable. On return, the variable refers to the printer associated with the specified printing session. The printer object is valid as long as the printing session is valid or the current printer hasn’t changed. You should not release this object without first retaining it.

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

func PMSessionSetCurrentPMPrinter(PMPrintSession, PMPrinter) -> OSStatus

Changes the current printer for a printing session.

func PMSessionGetCGGraphicsContext(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CGContext>?>) -> OSStatus

Obtains the Quartz graphics context for the current page in a printing session.

func PMSessionError(PMPrintSession) -> OSStatus

Obtains the result code for any error returned by the printing session.

func PMSessionSetError(PMPrintSession, OSStatus) -> OSStatus

Sets the value of the current result code for the specified printing session.

