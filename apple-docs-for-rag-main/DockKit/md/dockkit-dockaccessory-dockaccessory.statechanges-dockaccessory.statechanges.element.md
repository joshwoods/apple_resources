

- DockKit
- DockAccessory
- DockAccessory.StateChanges
-  DockAccessory.StateChanges.Element 

Type Alias

# DockAccessory.StateChanges.Element

A dock accessory state change.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
typealias Element = DockAccessory.StateChange
```

## See Also

### Iterating over state changes

struct Iterator

An object that allows iteration over dock accessory state changes.

func makeAsyncIterator() -> DockAccessory.StateChanges.Iterator

Creates and returns an iterator that traverses the list of dock accessory state changes.

