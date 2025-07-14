

- AppKit
-  NSController 

Class

# NSController

An abstract class that implements the NSEditor and NSEditorRegistration informal protocols required for controller classes.

macOS

``` source
class NSController
```

## Topics

### Managing editing

func objectDidBeginEditing(any NSEditor)

Invoked to inform the receiver that `editor` has uncommitted changes that can affect the receiver.

func objectDidEndEditing(any NSEditor)

Invoked to inform the receiver that `editor` has committed or discarded its changes.

func commitEditing() -> Bool

Causes the receiver to attempt to commit any pending edits, returning true if successful or no edits were pending.

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempts to commit any pending changes in known editors of the receiver.

func discardEditing()

Discards any pending changes by registered editors.

var isEditing: Bool

A Boolean value indicating if any editors are registered with the controller.

### Initializers

init()

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSObjectController
- NSUserDefaultsController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSEditorRegistration
- NSObjectProtocol

## See Also

### Core Controllers

class NSObjectController

A controller that can manage an object’s properties referenced by key-value paths.

