

- AppKit
- NSDocument
-  autosavingIsImplicitlyCancellable 

Instance Property

# autosavingIsImplicitlyCancellable

Returns a Boolean value that indicates whether you can cancel an in-progress autosave operation.

macOS 10.7+

``` source
@MainActor
var autosavingIsImplicitlyCancellable: Bool { get }
```

## Discussion

The value of this property is true if autosaving is in progress but nothing bad would happen if it were cancelled. For example, when periodic autosaving is being done only for crash protection, which doesn’t need to be done all of the time, this property is set to true. When autosaving is being done because the document is being closed, the property is set to false.

When the value is true, your document-writing code can invoke unblockUserInteraction() after recording the fact that changes to the document model made by the user should first cancel the rest of the writing. Your code that makes changes to the document model then must always do that cancellation first. If your writing code is implicitly cancelled in this way, it should set the NSError object passed by reference to the writing method to NSUserCancelledError in NSCocoaErrorDomain.

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

var autosavingFileType: String?

Returns the document type to use for an autosave operation.

