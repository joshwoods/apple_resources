

- AppKit
- NSForm
-  cell(at:) Deprecated

Instance Method

# cell(at:)

Returns the entry at the specified index.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func cell(at index: Int) -> Any!
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`index`  

The index of the desired entry.

## Return Value

The form cell object at the specified index.

## See Also

### Getting Cells and Indices

func indexOfCell(withTag: Int) -> Int

Returns the index of the entry whose tag is `tag`.

Deprecated

func indexOfSelectedItem() -> Int

Returns the index of the selected entry.

Deprecated

