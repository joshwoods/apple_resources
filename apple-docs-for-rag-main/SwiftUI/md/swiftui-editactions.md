

- SwiftUI
-  EditActions 

Structure

# EditActions

A set of edit actions on a collection of data that a view can offer to a user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EditActions
```

## Topics

### Getting edit operations

static var all: EditActions&lt;Data>

All the edit actions available on this collection.

static var all: EditActions&lt;Data>

All the edit actions available on this collection.

static var all: EditActions&lt;Data>

All the edit actions available on this collection.

static var all: EditActions&lt;Data>

All the edit actions available on this collection.

static var delete: EditActions&lt;Data>

An edit action that allows the user to delete one or more elements of a collection.

static var move: EditActions&lt;Data>

An edit action that allows the user to move elements of a collection.

### Creating an edit operation

init(rawValue: Int)

Creates a new set from a raw value.

let rawValue: Int

The raw value.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Editing a list

func moveDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is movable.

func deleteDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is deletable.

var editMode: Binding&lt;EditMode>?

An indication of whether the user can edit the contents of a view associated with this environment.

enum EditMode

A mode that indicates whether the user can edit a view’s content.

struct EditableCollectionContent

An opaque wrapper view that adds editing capabilities to a row in a list.

struct IndexedIdentifierCollection

A collection wrapper that iterates over the indices and identifiers of a collection together.

