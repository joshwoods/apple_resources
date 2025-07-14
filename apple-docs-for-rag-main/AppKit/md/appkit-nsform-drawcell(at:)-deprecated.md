

- AppKit
- NSForm
-  drawCell(at:) Deprecated

Instance Method

# drawCell(at:)

Displays the entry at the specified index.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func drawCell(at index: Int)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`index`  

The index of the entry to draw.

## Discussion

Because this method is called automatically whenever a cell needs drawing, you never need to invoke it explicitly. It is included in the API so you can override it if you subclass `NSFormCell`.

## See Also

### Related Documentation

func indexOfCell(withTag: Int) -> Int

Returns the index of the entry whose tag is `tag`.

Deprecated

func indexOfSelectedItem() -> Int

Returns the index of the selected entry.

Deprecated

