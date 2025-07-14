

- AppKit
- NSDocument
-  hasUnautosavedChanges 

Instance Property

# hasUnautosavedChanges

A Boolean value that indicates whether the document has changes that have not been autosaved.

macOS

``` source
@MainActor
var hasUnautosavedChanges: Bool { get }
```

## Discussion

The value of this property is true if the document has changes that have not been autosaved; otherwise, the value is false. A document has unsaved changes when the updateChangeCount(_:) method has been called since the last save.

## See Also

### Autosaving the Document

func checkAutosavingSafety() throws

Returns a Boolean value that indicates whether it is safe to autosave document changes.

func scheduleAutosaving()

Schedules periodic autosaving for the purpose of crash protection.

func autosave(withDelegate: Any?, didAutosave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Autosaves the document’s contents to an appropriate location in the file system.

func autosave(withImplicitCancellability: Bool, completionHandler: ((any Error)?) -> Void)

Autosaves the document’s contents to an appropriate file-system location, as needed.

var backupFileURL: URL?

The URL for the document’s backup file that was created during an autosave operation.

