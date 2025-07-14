

- UIKit
- UIDocument
- UIDocument.State
-  savingError 

Type Property

# savingError

There was an error in saving or reverting the document.

iOSiPadOSMac CatalystvisionOS

``` source
static var savingError: UIDocument.State { get }
```

## See Also

### Constants

static var normal: UIDocument.State

The document is open, editing is enabled, and there are no conflicts or errors associated with it.

static var closed: UIDocument.State

There was an error in reading the document.

static var inConflict: UIDocument.State

Conflicts exist for the document file located at the file URL.

static var editingDisabled: UIDocument.State

The document is busy and it isn’t currently safe for user edits.

static var progressAvailable: UIDocument.State

The document is being downloaded or uploaded and progress information is available.

