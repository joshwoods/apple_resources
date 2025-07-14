

- SwiftUI
- View
-  moveDisabled(\_:) 

Instance Method

# moveDisabled(\_:)

Adds a condition for whether the view’s view hierarchy is movable.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func moveDisabled(_ isDisabled: Bool) -> some View
```

## Mentioned in 

Making a view into a drag source

## See Also

### Editing a list

func deleteDisabled(Bool) -> some View

Adds a condition for whether the view’s view hierarchy is deletable.

var editMode: Binding&lt;EditMode>?

An indication of whether the user can edit the contents of a view associated with this environment.

enum EditMode

A mode that indicates whether the user can edit a view’s content.

struct EditActions

A set of edit actions on a collection of data that a view can offer to a user.

struct EditableCollectionContent

An opaque wrapper view that adds editing capabilities to a row in a list.

struct IndexedIdentifierCollection

A collection wrapper that iterates over the indices and identifiers of a collection together.

