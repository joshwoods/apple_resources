

- AppKit
-  NSEditor 

Protocol

# NSEditor

macOS

``` source
protocol NSEditor : NSObjectProtocol
```

## Topics

### Instance Methods

func commitEditing() -> Bool

**Required**

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

**Required**

func commitEditingWithoutPresentingError() throws

**Required**

func discardEditing()

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSArrayController
- NSCollectionViewItem
- NSController
- NSDictionaryController
- NSObjectController
- NSPageController
- NSSplitViewController
- NSTabViewController
- NSTitlebarAccessoryViewController
- NSTreeController
- NSUserDefaultsController
- NSViewController

## See Also

### Object Editing

protocol NSEditorRegistration

A set of methods that controllers can implement to enable an editor view to inform the controller when it has uncommitted changes.

