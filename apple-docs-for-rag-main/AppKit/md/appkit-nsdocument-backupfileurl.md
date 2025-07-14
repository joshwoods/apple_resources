

- AppKit
- NSDocument
-  backupFileURL 

Instance Property

# backupFileURL

The URL for the document’s backup file that was created during an autosave operation.

macOS 10.8+

``` source
nonisolated
var backupFileURL: URL? { get }
```

## Discussion

This property specifies the location of the backup file, if any. If a backup file cannot be created or is not needed, the value of this property is `nil`.

Starting in OS X v10.8, document versions can be preserved using a backup file created during an autosave operation, which supports document versioning. This property gives you access to the backup file’s URL.

Using an autosave backup file for preserving versions is efficient. This is because an NSDocument instance is able to use the byMoving option when it calls the replaceItem(at:options:) method. The document gets the value of this property twice during saving:

1.  Before calling the writeSafely(to:ofType:for:) method: This is to check whether using the replace-by-moving option is possible and, if not, to allow the system to preserve data by instead using copying.

2.  Within the writeSafely(to:ofType:for:) method: This is to discover where to put the backup file.

When you implement the writeSafely(to:ofType:for:) method with the NSDocument.SaveOperationType.saveOperation or NSDocument.SaveOperationType.autosaveInPlaceOperation operation type, you must check this property’s value. If it is not `nil`, move the previous contents of the file (that would be overwritten) to the URL’s location. The default implementation of writeSafely(to:ofType:for:) does this.

To create a backup file from within your custom implementation of the writeSafely(to:ofType:for:) method, call the FileManager method replaceItem(at:withItemAt:backupItemName:options:resultingItemURL:), using a backup item name of `[[self backupFileURL] lastPathComponent]` and an option of withoutDeletingBackupItem option. If your custom implementation is unable to keep the backup file, you must override this property and return `nil` to ensure that the document’s file gets correctly preserved before it gets overwritten.

The default implementation of the writeSafely(to:ofType:for:) method returns a non-`nil` value based on the value of `[self fileURL]`, but only if the document’s file needs to be preserved prior to saving or if the preservesVersions method returns false. Otherwise, it returns `nil`.

## See Also

### Autosaving the Document

func checkAutosavingSafety() throws

Returns a Boolean value that indicates whether it is safe to autosave document changes.

var hasUnautosavedChanges: Bool

A Boolean value that indicates whether the document has changes that have not been autosaved.

func scheduleAutosaving()

Schedules periodic autosaving for the purpose of crash protection.

func autosave(withDelegate: Any?, didAutosave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Autosaves the document’s contents to an appropriate location in the file system.

func autosave(withImplicitCancellability: Bool, completionHandler: ((any Error)?) -> Void)

Autosaves the document’s contents to an appropriate file-system location, as needed.

