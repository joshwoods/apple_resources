

- AppKit
- NSDocument
-  lastComponentOfFileName 

Instance Property

# lastComponentOfFileName

The name of the document seen by the user in AppleScript.

macOS

``` source
@MainActor
var lastComponentOfFileName: String { get set }
```

## Discussion

This property contains the document name used during scripting. Note that this name may be different than the name used in fileURL.

## See Also

### Related Documentation

var displayName: String!

The name of the document as displayed in the title bars of the document’s windows and in alert dialogs related to the document.

### Handling Script Commands

func handleClose(NSCloseCommand) -> Any?

Handles the Close AppleScript command by attempting to close the document.

func handlePrint(NSScriptCommand) -> Any?

Handles the Print AppleScript command by attempting to print the document.

func handleSave(NSScriptCommand) -> Any?

Handles the Save AppleScript command by attempting to save the document.

var objectSpecifier: NSScriptObjectSpecifier

Returns the object specifier that represents the document.

