

- AppKit
- NSDocument
-  preservesVersions 

Type Property

# preservesVersions

Returns whether the document subclass supports version management.

macOS 10.7+

``` source
@MainActor
class var preservesVersions: Bool { get }
```

## Return Value

true if the receiving subclass of NSDocument supports Versions; otherwise false.

## Discussion

The default implementation of this method returns `[self autosavesInPlace]`. You can override it and return false to declare that `NSDocument` should not preserve old document versions.

Returning false from this method disables version browsing and revertToSaved(_:), which rely on version preservation when autosaving in place. Returning true from this method when autosavesInPlace returns false will result in undefined behavior.

## See Also

### Configuring the Autosave Behavior

class var autosavesInPlace: Bool

Returns whether the receiver supports autosaving in place.

class var autosavesDrafts: Bool

A Boolean value that indicates whether the document subclass supports autosaving of drafts.

var autosavedContentsFileURL: URL?

The location of the most recently autosaved document contents.

var autosavingFileType: String?

Returns the document type to use for an autosave operation.

var autosavingIsImplicitlyCancellable: Bool

Returns a Boolean value that indicates whether you can cancel an in-progress autosave operation.

