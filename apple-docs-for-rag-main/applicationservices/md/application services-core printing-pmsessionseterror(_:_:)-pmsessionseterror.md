

- Application Services
- Core Printing
-  PMSessionSetError(\_:\_:) 

Function

# PMSessionSetError(\_:\_:)

Sets the value of the current result code for the specified printing session.

macOS 10.0+

``` source
func PMSessionSetError(
    _ printSession: PMPrintSession,
    _ printError: OSStatus
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session whose result code you want to set.

`printError`  

The result code you want to set. This result code is returned by the `PMSessionError` function.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

You can use this function to terminate a printing session if your application encounters any errors inside the print loop. Typically, this function is used by an application’s idle function. The idle function isn’t called in macOS, so this usage is not available.

## See Also

### Accessing Data in Printing Session Objects

func PMSessionGetDataFromSession(PMPrintSession, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>) -> OSStatus

Obtains application-specific data previously stored in a printing session object.

func PMSessionSetDataInSession(PMPrintSession, CFString, CFTypeRef) -> OSStatus

Stores your application-specific data in a printing session object.

func PMSessionGetCurrentPrinter(PMPrintSession, UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Obtains the current printer associated with a printing session.

func PMSessionSetCurrentPMPrinter(PMPrintSession, PMPrinter) -> OSStatus

Changes the current printer for a printing session.

func PMSessionGetCGGraphicsContext(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CGContext>?>) -> OSStatus

Obtains the Quartz graphics context for the current page in a printing session.

func PMSessionError(PMPrintSession) -> OSStatus

Obtains the result code for any error returned by the printing session.

