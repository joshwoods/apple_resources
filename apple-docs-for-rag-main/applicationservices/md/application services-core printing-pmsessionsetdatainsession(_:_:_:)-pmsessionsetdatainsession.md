

- Application Services
- Core Printing
-  PMSessionSetDataInSession(\_:\_:\_:) 

Function

# PMSessionSetDataInSession(\_:\_:\_:)

Stores your application-specific data in a printing session object.

macOS 10.0+

``` source
func PMSessionSetDataInSession(
    _ printSession: PMPrintSession,
    _ key: CFString,
    _ data: CFTypeRef
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session in which you want to store application-specific data.

`key`  

A key that uniquely identifies the data being added. This key is required to retrieve the data using the function PMSessionGetDataFromSession(_:_:_:).

`data`  

The data to be stored in the printing session.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

## See Also

### Accessing Data in Printing Session Objects

func PMSessionGetDataFromSession(PMPrintSession, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>) -> OSStatus

Obtains application-specific data previously stored in a printing session object.

func PMSessionGetCurrentPrinter(PMPrintSession, UnsafeMutablePointer&lt;PMPrinter?>) -> OSStatus

Obtains the current printer associated with a printing session.

func PMSessionSetCurrentPMPrinter(PMPrintSession, PMPrinter) -> OSStatus

Changes the current printer for a printing session.

func PMSessionGetCGGraphicsContext(PMPrintSession, UnsafeMutablePointer&lt;Unmanaged&lt;CGContext>?>) -> OSStatus

Obtains the Quartz graphics context for the current page in a printing session.

func PMSessionError(PMPrintSession) -> OSStatus

Obtains the result code for any error returned by the printing session.

func PMSessionSetError(PMPrintSession, OSStatus) -> OSStatus

Sets the value of the current result code for the specified printing session.

