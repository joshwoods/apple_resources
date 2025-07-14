

- AppKit
- NSTextFinderClient
-  isEditable 

Instance Property

# isEditable

Returns whether the text is editable.

macOS

``` source
optional var isEditable: Bool { get }
```

## Discussion

The text finder uses this property to validate actions. If is it not implemented, the value is assumed to be true .

