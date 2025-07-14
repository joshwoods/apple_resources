

- AppKit
- NSForm
-  insertEntry(\_:at:) Deprecated

Instance Method

# insertEntry(\_:at:)

Inserts an entry with the specified title into the receiver.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func insertEntry(
    _ title: String,
    at index: Int
) -> NSFormCell!
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`title`  

The title for the new form entry.

`index`  

The zero-based index at which to insert the entry.

## Return Value

The form cell object that was created for the entry.

## Discussion

The new entry has no tag, target, or action, but is enabled and editable.

## See Also

### Adding and Removing Entries

func addEntry(String) -> NSFormCell

Adds a new entry to the end of the receiver and gives it the specified title.

Deprecated

func removeEntry(at: Int)

Removes and releases the entry at the specified index.

Deprecated

