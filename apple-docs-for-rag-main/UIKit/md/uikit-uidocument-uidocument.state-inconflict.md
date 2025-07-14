

- UIKit
- UIDocument
- UIDocument.State
-  inConflict 

Type Property

# inConflict

Conflicts exist for the document file located at the file URL.

iOSiPadOSMac CatalystvisionOS

``` source
static var inConflict: UIDocument.State { get }
```

## Discussion

You can access these conflicting document versions by calling the otherVersionsOfItem(at:) class method of the NSFileVersion class. This method returns an array of NSFileVersion objects. You can then resolve the conflicting versions — for example, programmatically attempt to merge the versions or present the document versions to a person and request them to pick one.

## See Also

### Constants

static var normal: UIDocument.State

The document is open, editing is enabled, and there are no conflicts or errors associated with it.

static var closed: UIDocument.State

There was an error in reading the document.

static var savingError: UIDocument.State

There was an error in saving or reverting the document.

static var editingDisabled: UIDocument.State

The document is busy and it isn’t currently safe for user edits.

static var progressAvailable: UIDocument.State

The document is being downloaded or uploaded and progress information is available.

