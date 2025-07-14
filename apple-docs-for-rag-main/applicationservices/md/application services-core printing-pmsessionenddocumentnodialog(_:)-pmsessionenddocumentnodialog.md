

- Application Services
- Core Printing
-  PMSessionEndDocumentNoDialog(\_:) 

Function

# PMSessionEndDocumentNoDialog(\_:)

Ends a print job started by calling the function PMSessionBeginCGDocumentNoDialog(_:_:_:) or PMSessionBeginDocumentNoDialog.

macOS 10.2+

``` source
func PMSessionEndDocumentNoDialog(_ printSession: PMPrintSession) -> OSStatus
```

## Parameters 

`printSession`  

The current printing session. On return, the printing session is no longer valid; however, you must still call the function PMRelease(_:) to release the object.

## Return Value

A result code. See Result Codes.

## Discussion

This function is similar to the function `PMSessionEndDocument` except that the printing status dialog is suppressed.

This function is used to end a print job, and it should be called within your application’s print loop after the call to the function `PMSessionEndPageNoDialog` and before releasing the printing session. The same printing session that is created by the function `PMCreateSession` for the Print dialog should be used for the print loop.

The function `PMSessionEndDocumentNoDialog` must be called after its corresponding `Begin` function (PMSessionBeginCGDocumentNoDialog(_:_:_:) or PMSessionBeginDocumentNoDialog). If the `Begin` function returns `noErr`, the function `PMSessionEndDocument` must be called, even if errors occur within the scope of the `Begin` and `End` functions. You should not call `PMSessionEndDocumentNoDialog` if the `Begin` function returns an error.

## See Also

### Print Loop Functions

func PMSessionBeginCGDocumentNoDialog(PMPrintSession, PMPrintSettings, PMPageFormat) -> OSStatus

Begins a print job that draws into a Quartz graphics context and suppresses the printing status dialog.

func PMSessionBeginPageNoDialog(PMPrintSession, PMPageFormat?, UnsafePointer&lt;PMRect>?) -> OSStatus

Starts a new page for printing in the specified printing session and suppresses the printing status dialog.

func PMSessionEndPageNoDialog(PMPrintSession) -> OSStatus

Indicates the end of drawing the current page for the specified printing session.

