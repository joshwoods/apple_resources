

- AppKit
- NSForm
-  selectText(at:) Deprecated

Instance Method

# selectText(at:)

Selects the entry at the specified index.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func selectText(at index: Int)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`index`  

The index of the entry to select. If the specified index is invalid, this method does nothing.

