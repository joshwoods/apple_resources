

- AppKit
-  NSArrayController 

Class

# NSArrayController

A bindings-compatible controller that manages a collection of objects.

macOS

``` source
class NSArrayController
```

## Overview

Typically the collection that an NSArrayController manages is an array, however, if the controller manages a relationship of a managed object (see NSManagedObject) the collection may be a set. NSArrayController provides selection management and sorting capabilities.

## Topics

### Managing Sort Descriptors

var sortDescriptors: [NSSortDescriptor]

An array of NSSortDescriptor objects, used by the receiver to arrange its content.

### Arranging Objects

func arrange([Any]) -> [Any]

Returns a given array, appropriately sorted and filtered.

var arrangedObjects: Any

An array containing the receiver’s content objects arranged using arrange(_:).

func rearrangeObjects()

Triggers filtering of the receiver’s content.

### Managing Content

func add(Any?)

Creates and adds a new object to the receiver’s content and arranged objects.

### Selection Attributes

var avoidsEmptySelection: Bool

A Boolean value that indicates whether the receiver requires that the content array attempt to maintain a selection

var preservesSelection: Bool

A Boolean value that indicates whether the receiver will attempt to preserve the current selection when the content changes

var alwaysUsesMultipleValuesMarker: Bool

A Boolean value that indicates whether the receiver always returns the multiple values marker when multiple objects are selected

### Managing selections

var selectionIndex: Int

The index of the first object in the receiver’s selection

func setSelectionIndex(Int) -> Bool

Sets the receiver’s selection to the given index, and returns a Boolean value that indicates whether the selection was changed.

var selectsInsertedObjects: Bool

A Boolean value that indicates whether the receiver automatically selects inserted objects

func setSelectionIndexes(IndexSet) -> Bool

Sets the receiver’s selection indexes and returns a Boolean value that indicates whether the selection changed.

var selectionIndexes: IndexSet

An index set containing the indexes of the receiver’s currently selected objects in the content array

func addSelectionIndexes(IndexSet) -> Bool

Adds the objects at the specified indexes in the receiver’s content array to the current selection, returning true if the selection was changed.

func removeSelectionIndexes(IndexSet) -> Bool

Removes the object as the specified `indexes` from the receiver’s current selection, returning true if the selection was changed.

func setSelectedObjects([Any]) -> Bool

Sets `objects` as the receiver’s current selection, returning true if the selection was changed.

var selectedObjects: [Any]!

An array containing the receiver’s selected objects

func addSelectedObjects([Any]) -> Bool

Adds `objects` from the receiver’s content array to the current selection, returning true if the selection was changed.

func removeSelectedObjects([Any]) -> Bool

Removes `objects` from the receiver’s current selection, returning true if the selection was changed.

func selectNext(Any?)

Selects the next object, relative to the current selection, in the receiver’s arranged content.

var canSelectNext: Bool

A Boolean value indicating whether the next object, relative to the current selection, in the receiver’s content array can be selected

func selectPrevious(Any?)

Selects the previous object, relative to the current selection, in the receiver’s arranged content.

var canSelectPrevious: Bool

A Boolean value indicating whether the previous object, relative to the current selection, in the receiver’s content array can be selected

### Inserting

var canInsert: Bool

Returns a Boolean value that indicates whether an object can be inserted into the receiver’s content collection.

func insert(Any?)

Creates a new object and inserts it into the receiver’s content array.

### Adding and Removing Objects

func addObject(Any)

Adds `object` to the receiver’s content collection and the arranged objects array.

func add(contentsOf: [Any])

Adds `objects` to the receiver’s content collection.

func insert(Any, atArrangedObjectIndex: Int)

Inserts `object` into the receiver’s arranged objects array at the location specified by `index`, and adds it to the receiver’s content collection.

func insert(contentsOf: [Any], atArrangedObjectIndexes: IndexSet)

Inserts `object`s into the receiver’s arranged objects array at the locations specified in `indexes`, and adds it to the receiver’s content collection.

func remove(atArrangedObjectIndex: Int)

Removes the object at the specified `index` in the receiver’s arranged objects from the receiver’s content array.

func remove(atArrangedObjectIndexes: IndexSet)

Removes the objects at the specified `indexes` in the receiver’s arranged objects from the content array.

func remove(Any?)

Removes the receiver’s selected objects from the content collection.

func removeObject(Any)

Removes `object` from the receiver’s content collection.

func remove(contentsOf: [Any])

Removes `objects` from the receiver’s content collection.

### Filtering Content

var clearsFilterPredicateOnInsertion: Bool

A Boolean value that indicates whether the receiver automatically clears an existing filter predicate when new items are inserted or added to the content

var filterPredicate: NSPredicate?

A predicate used by the receiver to filter the array controller contents

### Automatic Content Rearranging

var automaticallyRearrangesObjects: Bool

A Boolean that indicates if the receiver automatically rearranges its content to correspond to the current sort descriptors and filter predicates

var automaticRearrangementKeyPaths: [String]?

An array of key paths that trigger automatic content sorting or filtering

func didChangeArrangementCriteria()

Invoked when any criteria for arranging objects change.

## Relationships

### Inherits From

- NSObjectController

### Inherited By

- NSDictionaryController

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

