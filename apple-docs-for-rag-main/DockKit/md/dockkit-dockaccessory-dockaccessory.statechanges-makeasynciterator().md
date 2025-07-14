

- DockKit
- DockAccessory
- DockAccessory.StateChanges
-  makeAsyncIterator() 

Instance Method

# makeAsyncIterator()

Creates and returns an iterator that traverses the list of dock accessory state changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
func makeAsyncIterator() -> DockAccessory.StateChanges.Iterator
```

## See Also

### Iterating over state changes

struct Iterator

An object that allows iteration over dock accessory state changes.

typealias Element

A dock accessory state change.

