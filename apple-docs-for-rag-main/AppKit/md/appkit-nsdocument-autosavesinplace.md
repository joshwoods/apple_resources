

- AppKit
- NSDocument
-  autosavesInPlace 

Type Property

# autosavesInPlace

Returns whether the receiver supports autosaving in place.

macOS 10.7+

``` source
nonisolated
class var autosavesInPlace: Bool { get }
```

## Return Value

true if the receiver supports autosaving in place; false otherwise.

## Discussion

The default implementation of this method returns false. You can override it and return true to declare that your subclass of `NSDocument` can do autosaving in place. You should not invoke this method to find out whether autosaving in place is actually being done at any particular moment. You should instead use the NSDocument.SaveOperationType parameter that the system passes to your overrides of save and write methods.

AppKit invokes this method at a variety of times, and not always on the main thread. For example, autosave(withImplicitCancellability:completionHandler:) invokes this method as part of determining whether the autosaving will be performed in place (NSDocument.SaveOperationType.autosaveInPlaceOperation) or in a separate autosave directory (NSDocument.SaveOperationType.autosaveElsewhereOperation). As another example, the canClose(withDelegate:shouldClose:contextInfo:) method and the NSDocumentController machinery for handling unsaved changes at app termination time both invoke this method as part of determining whether alerts about unsaved changes should be presented to the user.

## See Also

### Configuring the Autosave Behavior

class var autosavesDrafts: Bool

A Boolean value that indicates whether the document subclass supports autosaving of drafts.

class var preservesVersions: Bool

Returns whether the document subclass supports version management.

var autosavedContentsFileURL: URL?

The location of the most recently autosaved document contents.

var autosavingFileType: String?

Returns the document type to use for an autosave operation.

var autosavingIsImplicitlyCancellable: Bool

Returns a Boolean value that indicates whether you can cancel an in-progress autosave operation.

