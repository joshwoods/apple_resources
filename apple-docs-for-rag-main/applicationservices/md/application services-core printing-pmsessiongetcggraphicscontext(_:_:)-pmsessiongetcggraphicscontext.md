

- Application Services
- Core Printing
-  PMSessionGetCGGraphicsContext(\_:\_:) 

Function

# PMSessionGetCGGraphicsContext(\_:\_:)

Obtains the Quartz graphics context for the current page in a printing session.

macOS 10.4+

``` source
func PMSessionGetCGGraphicsContext(
    _ printSession: PMPrintSession,
    _ context: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSession`  

The printing session whose Quartz graphics context you want to obtain.

`context`  

A pointer to your CGContext variable. On return, the variable refers to the Quartz graphics context for the current page in the specified printing session. The context’s origin is at the lower-left corner of the sheet of paper, not the imageable area. You should not release the context without first retaining it. The context is valid only for the current page; you should not retain it beyond the end of the page.

## Return Value

A result code. See Result Codes.

## Discussion

If you’re using Quartz 2D to draw the content for a print job, after each call to `PMSessionBeginPage` you should call `PMSessionGetCGGraphicsContext` to obtain the Quartz graphics context for the current page. Note that before you can use the function `PMSessionGetCGGraphicsContext`, you must have called `PMSessionBeginCGDocument` or PMSessionBeginCGDocumentNoDialog(_:_:_:) instead of PMSessionBeginDocument or PMSessionBeginDocumentNoDialog.

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

func PMSessionError(PMPrintSession) -> OSStatus

Obtains the result code for any error returned by the printing session.

func PMSessionSetError(PMPrintSession, OSStatus) -> OSStatus

Sets the value of the current result code for the specified printing session.

