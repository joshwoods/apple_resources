

- SwiftUI
-  EditableCollectionContent 

Structure

# EditableCollectionContent

An opaque wrapper view that adds editing capabilities to a row in a list.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EditableCollectionContent
```

## Overview

You don’t use this type directly. Instead SwiftUI creates this type on your behalf.

## Relationships

### Conforms To

- Copyable
- View

  Conforms when `Content` conforms to `View`, `Data` conforms to `Copyable`, and `Data` conforms to `Escapable`.

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

struct EditActions

A set of edit actions on a collection of data that a view can offer to a user.

struct IndexedIdentifierCollection

A collection wrapper that iterates over the indices and identifiers of a collection together.

