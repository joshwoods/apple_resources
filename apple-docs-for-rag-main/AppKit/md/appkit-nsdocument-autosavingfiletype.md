

- AppKit
- NSDocument
-  autosavingFileType 

Instance Property

# autosavingFileType

Returns the document type to use for an autosave operation.

macOS

``` source
nonisolated
var autosavingFileType: String? { get }
```

## Discussion

This properties contains a string that identifies the document type for autosave files. The default implementation just returns the value provided by the fileType property. You can override this property and return `nil` to completely disable autosaving of individual documents (because the NSDocumentController object does not call the autosave(withDelegate:didAutosave:contextInfo:) method of a document that has no autosaving file type). You can also override it if your app defines a document type that is specifically designed for autosaving, for example, one that efficiently represents document content changes instead of complete document contents.

Overriding this property can result in incorrect behavior during reopening of autosaved documents. The `NSDocument` method init(for:withContentsOf:ofType:), which is invoked during reopening of autosaved documents after a crash, takes two URLs, but only the type name of the autosaved contents file. The default implementation updates the fileType property with that type name, but that may not be the right thing to do if this property contains something other than fileType during document autosaving. If you override `autosavingFileType`, you probably need to override init(for:withContentsOf:ofType:) too, and make the override update fileType with the type of the actual document file, after invoking `super`. See TextEdit’s `Document` class for an example of how to do this.

## See Also

### Configuring the Autosave Behavior

class var autosavesInPlace: Bool

Returns whether the receiver supports autosaving in place.

class var autosavesDrafts: Bool

A Boolean value that indicates whether the document subclass supports autosaving of drafts.

class var preservesVersions: Bool

Returns whether the document subclass supports version management.

var autosavedContentsFileURL: URL?

The location of the most recently autosaved document contents.

var autosavingIsImplicitlyCancellable: Bool

Returns a Boolean value that indicates whether you can cancel an in-progress autosave operation.

