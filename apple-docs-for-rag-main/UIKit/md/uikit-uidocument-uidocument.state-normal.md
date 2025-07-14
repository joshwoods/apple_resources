

- UIKit
- UIDocument
- UIDocument.State
-  normal 

Type Property

# normal

The document is open, editing is enabled, and there are no conflicts or errors associated with it.

iOSiPadOSMac CatalystvisionOS

``` source
static var normal: UIDocument.State { get }
```

## See Also

### Constants

static var closed: UIDocument.State

There was an error in reading the document.

static var inConflict: UIDocument.State

Conflicts exist for the document file located at the file URL.

static var savingError: UIDocument.State

There was an error in saving or reverting the document.

static var editingDisabled: UIDocument.State

The document is busy and it isn’t currently safe for user edits.

static var progressAvailable: UIDocument.State

The document is being downloaded or uploaded and progress information is available.

