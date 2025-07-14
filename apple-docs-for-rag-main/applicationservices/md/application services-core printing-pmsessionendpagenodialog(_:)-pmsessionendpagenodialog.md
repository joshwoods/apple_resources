

- Application Services
- Core Printing
-  PMSessionEndPageNoDialog(\_:) 

Function

# PMSessionEndPageNoDialog(\_:)

Indicates the end of drawing the current page for the specified printing session.

macOS 10.2+

``` source
func PMSessionEndPageNoDialog(_ printSession: PMPrintSession) -> OSStatus
```

## Parameters 

`printSession`  

The printing session that provides a context for the print job.

## Return Value

A result code. See Result Codes.

## Discussion

This function is similar to the function `PMSessionEndPage` except that the printing status dialog is suppressed.

You must call this function between the creation and release of a printing session. See the function PMCreateSession(_:). You must call the functions `PMSessionBeginPageNoDialog` and `PMSessionEndPageNoDialog` within the scope of calls to the `Begin` print job function (PMSessionBeginCGDocumentNoDialog(_:_:_:)) and the `End` print job function (PMSessionEndDocumentNoDialog(_:)).

If the function `PMSessionBeginPageNoDialog` returns `noErr`, you must later call the function `PMSessionEndPageNoDialog`, even if errors occur within the scope of `PMSessionBeginPageNoDialog` and `PMSessionEndPageNoDialog`. You should not call `PMSessionEndPageNoDialog` if `PMSessionBeginPageNoDialog` returns an error.

## See Also

### Print Loop Functions

func PMSessionBeginCGDocumentNoDialog(PMPrintSession, PMPrintSettings, PMPageFormat) -> OSStatus

Begins a print job that draws into a Quartz graphics context and suppresses the printing status dialog.

func PMSessionEndDocumentNoDialog(PMPrintSession) -> OSStatus

Ends a print job started by calling the function PMSessionBeginCGDocumentNoDialog(_:_:_:) or PMSessionBeginDocumentNoDialog.

func PMSessionBeginPageNoDialog(PMPrintSession, PMPageFormat?, UnsafePointer&lt;PMRect>?) -> OSStatus

Starts a new page for printing in the specified printing session and suppresses the printing status dialog.

