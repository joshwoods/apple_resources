

- AppKit
- NSArrayController
-  setSelectionIndexes(\_:) 

Instance Method

# setSelectionIndexes(\_:)

Sets the receiver’s selection indexes and returns a Boolean value that indicates whether the selection changed.

macOS

``` source
func setSelectionIndexes(_ indexes: IndexSet) -> Bool
```

## Parameters 

`indexes`  

The set of selection indexes for the receiver.

## Return Value

true if the selection was changed, otherwise false.

## Discussion

Attempting to change the selection may cause a commitEditing() message which fails, thus denying the selection change.

To select all the receiver’s objects, indexes should be an index set with indexes `[0...count -1]`. To deselect all indexes, pass an empty index set.

## See Also

### Managing selections

var selectionIndex: Int

The index of the first object in the receiver’s selection

func setSelectionIndex(Int) -> Bool

Sets the receiver’s selection to the given index, and returns a Boolean value that indicates whether the selection was changed.

var selectsInsertedObjects: Bool

A Boolean value that indicates whether the receiver automatically selects inserted objects

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

