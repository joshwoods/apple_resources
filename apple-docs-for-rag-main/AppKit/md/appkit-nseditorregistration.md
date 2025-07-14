

- AppKit
-  NSEditorRegistration 

Protocol

# NSEditorRegistration

A set of methods that controllers can implement to enable an editor view to inform the controller when it has uncommitted changes.

macOS

``` source
protocol NSEditorRegistration : NSObjectProtocol
```

## Overview

An implementor is responsible for tracking which editors have uncommitted changes, and sending those editors commitEditing and discardEditing messages, as appropriate, to force the editor to submit, or discard, their values.

NSController provides an implementation of this informal protocol. You would implement this protocol if you wanted to provide your own controller class without subclassing NSController.

## Topics

### Instance Methods

func objectDidBeginEditing(any NSEditor)

func objectDidEndEditing(any NSEditor)

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSArrayController
- NSController
- NSDictionaryController
- NSDocument
- NSObjectController
- NSPersistentDocument
- NSTreeController
- NSUserDefaultsController

## See Also

### Protocols

NSAccessibility

A legacy, informal protocol that Apple doesn’t recommend for active use.

NSEditor

A set of methods that controllers and UI elements can implement to manage editing.

protocol NSInputServiceProvider

protocol NSInputServerMouseTracker

protocol NSDrawerDelegate

A set of methods that drawer delegates implement to open, close, and resize the drawer.

Deprecated

