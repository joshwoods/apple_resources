

- AppKit
- NSDocument
-  autosavesDrafts 

Type Property

# autosavesDrafts

A Boolean value that indicates whether the document subclass supports autosaving of drafts.

macOS 10.8+

``` source
@MainActor
class var autosavesDrafts: Bool { get }
```

## Return Value

true if the receiving subclass of NSDocument supports autosaving of drafts; otherwise, false.

## Discussion

The system expects that an NSDocument subclass that returns true from this property can properly handle save operations that use the NSDocument.SaveOperationType.autosaveAsOperation save operation type.

The default implementation of this property returns true. To opt out of autosaving in your NSDocument subclass, override this property to return false.

AppKit invokes this property at various times. For example, when calling the updateChangeCount(_:) method with NSDocument.ChangeType.changeDone, but without the NSDocument.ChangeType.changeDiscardable change type, `NSDocument` uses NSDocument.SaveOperationType.autosaveAsOperation on the next autosave. The operation writes the document’s contents to a new file or file package, then changes the document’s current location to point to the new file or file package.

Don’t invoke this property to find out whether autosaving of a draft might occur.

## See Also

### Configuring the Autosave Behavior

class var autosavesInPlace: Bool

Returns whether the receiver supports autosaving in place.

class var preservesVersions: Bool

Returns whether the document subclass supports version management.

var autosavedContentsFileURL: URL?

The location of the most recently autosaved document contents.

var autosavingFileType: String?

Returns the document type to use for an autosave operation.

var autosavingIsImplicitlyCancellable: Bool

Returns a Boolean value that indicates whether you can cancel an in-progress autosave operation.

