

- AppKit
- NSDocument
-  handlePrint(\_:) 

Instance Method

# handlePrint(\_:)

Handles the Print AppleScript command by attempting to print the document.

macOS

``` source
@MainActor
func handlePrint(_ command: NSScriptCommand) -> Any?
```

## Parameters 

`command`  

An AppleScript command object.

## Discussion

Extracts Print command arguments from the `command` object and uses them to determine how to print the document—specifically, any print settings and whether to show the Print dialog. A Print AppleScript command may specify more than one document to print. If so, a message is sent to each document.

## See Also

### Handling Script Commands

func handleClose(NSCloseCommand) -> Any?

Handles the Close AppleScript command by attempting to close the document.

func handleSave(NSScriptCommand) -> Any?

Handles the Save AppleScript command by attempting to save the document.

var objectSpecifier: NSScriptObjectSpecifier

Returns the object specifier that represents the document.

var lastComponentOfFileName: String

The name of the document seen by the user in AppleScript.

