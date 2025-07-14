

- AppKit
- NSDocument
-  handleSave(\_:) 

Instance Method

# handleSave(\_:)

Handles the Save AppleScript command by attempting to save the document.

macOS

``` source
@MainActor
func handleSave(_ command: NSScriptCommand) -> Any?
```

## Parameters 

`command`  

An AppleScript command object.

## Discussion

Extracts Save command arguments from the `command` object and uses them to determine the file in which to save the document and the file type.

## See Also

### Handling Script Commands

func handleClose(NSCloseCommand) -> Any?

Handles the Close AppleScript command by attempting to close the document.

func handlePrint(NSScriptCommand) -> Any?

Handles the Print AppleScript command by attempting to print the document.

var objectSpecifier: NSScriptObjectSpecifier

Returns the object specifier that represents the document.

var lastComponentOfFileName: String

The name of the document seen by the user in AppleScript.

