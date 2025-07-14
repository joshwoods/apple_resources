

- UIKit
- UIDocument
-  UIDocument.State 

Structure

# UIDocument.State

Constants that specify the document state.

iOSiPadOSMac CatalystvisionOS

``` source
struct State
```

## Overview

A UIDocument object stores the current state of the document in the documentState property. To receive notifications about changes in document state, observe the stateChangedNotification notification.

## Topics

### Constants

static var normal: UIDocument.State

The document is open, editing is enabled, and there are no conflicts or errors associated with it.

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

### Initializers

init(rawValue: UInt)

Creates a document state structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

enum ChangeKind

Constants that specify the kind of change to a document.

enum SaveOperation

Constants that specify the type of save operation.

class let userActivityURLKey: String

The key that identifies the document associated with a user activity.

