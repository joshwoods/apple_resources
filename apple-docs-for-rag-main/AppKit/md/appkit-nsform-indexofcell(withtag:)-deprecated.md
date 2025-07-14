

- AppKit
- NSForm
-  indexOfCell(withTag:) Deprecated

Instance Method

# indexOfCell(withTag:)

Returns the index of the entry whose tag is `tag`.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func indexOfCell(withTag tag: Int) -> Int
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`tag`  

The tag of the desired entry.

## See Also

### Related Documentation

var tag: Int

A tag for identifying the cell.

### Getting Cells and Indices

func indexOfSelectedItem() -> Int

Returns the index of the selected entry.

Deprecated

func cell(at: Int) -> Any!

Returns the entry at the specified index.

Deprecated

