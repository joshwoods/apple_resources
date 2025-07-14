

- AppKit
- NSForm
-  addEntry(\_:) Deprecated

Instance Method

# addEntry(\_:)

Adds a new entry to the end of the receiver and gives it the specified title.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func addEntry(_ title: String) -> NSFormCell
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`title`  

The title for the new form entry.

## Return Value

The form cell object that was created for the entry.

## Discussion

The new entry has no tag, target, or action, but is enabled and editable.

## See Also

### Related Documentation

var action: Selector?

Returns the receiver’s action-message selector.

var target: AnyObject?

Returns the receiver’s target object.

var isEnabled: Bool

A Boolean value indicating whether the cell is currently enabled.

var isEditable: Bool

A Boolean value indicating whether the cell is editable.

var tag: Int

Returns the receiver’s tag.

Form Programming Topics

Matrix Programming Guide

### Adding and Removing Entries

func insertEntry(String, at: Int) -> NSFormCell!

Inserts an entry with the specified title into the receiver.

Deprecated

func removeEntry(at: Int)

Removes and releases the entry at the specified index.

Deprecated

