

- AppKit
- NSDocument
-  objectSpecifier 

Instance Property

# objectSpecifier

Returns the object specifier that represents the document.

macOS

``` source
@MainActor
var objectSpecifier: NSScriptObjectSpecifier { get }
```

## Return Value

The document object specifier.

## Discussion

An object specifier represents an AppleScript reference form, which is a natural-language expression such as `words 10 through 20` or `front document`. During script processing, an object contained by a document (such as the `second paragraph` or the `third rectangle`) may need to specify its container (the document).

## See Also

### Handling Script Commands

func handleClose(NSCloseCommand) -> Any?

Handles the Close AppleScript command by attempting to close the document.

func handlePrint(NSScriptCommand) -> Any?

Handles the Print AppleScript command by attempting to print the document.

func handleSave(NSScriptCommand) -> Any?

Handles the Save AppleScript command by attempting to save the document.

var lastComponentOfFileName: String

The name of the document seen by the user in AppleScript.

