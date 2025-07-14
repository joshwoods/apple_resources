

- AppKit
- NSDocument
-  autosavedContentsFileURL 

Instance Property

# autosavedContentsFileURL

The location of the most recently autosaved document contents.

macOS

``` source
nonisolated
var autosavedContentsFileURL: URL? { get set }
```

## Discussion

Use this property to specify the location where you want the document to store autosave files. The URL you specify should specify an absolute path, not a relative path.

## See Also

### Configuring the Autosave Behavior

class var autosavesInPlace: Bool

Returns whether the receiver supports autosaving in place.

class var autosavesDrafts: Bool

A Boolean value that indicates whether the document subclass supports autosaving of drafts.

class var preservesVersions: Bool

Returns whether the document subclass supports version management.

var autosavingFileType: String?

Returns the document type to use for an autosave operation.

var autosavingIsImplicitlyCancellable: Bool

Returns a Boolean value that indicates whether you can cancel an in-progress autosave operation.

