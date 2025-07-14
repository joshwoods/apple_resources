

- AppKit
- NSForm
-  indexOfSelectedItem() Deprecated

Instance Method

# indexOfSelectedItem()

Returns the index of the selected entry.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func indexOfSelectedItem() -> Int
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Return Value

The index of the selected entry, or `-1` if no entry is selected.

## See Also

### Getting Cells and Indices

func indexOfCell(withTag: Int) -> Int

Returns the index of the entry whose tag is `tag`.

Deprecated

func cell(at: Int) -> Any!

Returns the entry at the specified index.

Deprecated

