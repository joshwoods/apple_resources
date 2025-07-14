

- UIKit
- UIDocument
- UIDocument.State
-  editingDisabled 

Type Property

# editingDisabled

The document is busy and it isn’t currently safe for user edits.

iOSiPadOSMac CatalystvisionOS

``` source
static var editingDisabled: UIDocument.State { get }
```

## Discussion

This state is set just before UIDocument calls the disableEditing() method. It calls enableEditing() when it becomes safe to edit again. UIDocument also sets this state when an error prevents the reverting of a document.

## See Also

### Constants

static var normal: UIDocument.State

The document is open, editing is enabled, and there are no conflicts or errors associated with it.

static var closed: UIDocument.State

There was an error in reading the document.

static var inConflict: UIDocument.State

Conflicts exist for the document file located at the file URL.

static var savingError: UIDocument.State

There was an error in saving or reverting the document.

static var progressAvailable: UIDocument.State

The document is being downloaded or uploaded and progress information is available.

