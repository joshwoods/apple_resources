

- Application Services
- Core Printing
-  PMSessionGetDataFromSession(\_:\_:\_:) 

Function

# PMSessionGetDataFromSession(\_:\_:\_:)

Obtains application-specific data previously stored in a printing session object.

macOS 10.0+

``` source
func PMSessionGetDataFromSession(
    _ printSession: PMPrintSession,
    _ key: CFString,
    _ data: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session whose data you want to obtain.

`key`  

The key that uniquely identifies the data to be retrieved. You specify this key when you store the data using the function PMSessionSetDataInSession(_:_:_:).

`data`  

A pointer to your CFTypeRef variable. On return, the variable refers to the data retrieved from the printing session.

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:).

## See Also

### Accessing Data in Printing Session Objects

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

func PMSessionSetError(PMPrintSession, OSStatus) -> OSStatus

Sets the value of the current result code for the specified printing session.

