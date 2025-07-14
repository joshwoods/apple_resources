

- AppKit
- NSForm
-  removeEntry(at:) Deprecated

Instance Method

# removeEntry(at:)

Removes and releases the entry at the specified index.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func removeEntry(at index: Int)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`index`  

The zero-based index identifying the desired entry.

## Discussion

If the specified index is invalid, this method does nothing.

## See Also

### Adding and Removing Entries

func addEntry(String) -> NSFormCell

Adds a new entry to the end of the receiver and gives it the specified title.

Deprecated

func insertEntry(String, at: Int) -> NSFormCell!

Inserts an entry with the specified title into the receiver.

Deprecated

