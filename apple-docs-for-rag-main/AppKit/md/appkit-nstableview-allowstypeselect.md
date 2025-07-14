

- AppKit
- NSTableView
-  allowsTypeSelect 

Instance Property

# allowsTypeSelect

A Boolean value indicating whether the table view allows the user to type characters to select rows.

macOS 10.5+

``` source
@MainActor
var allowsTypeSelect: Bool { get set }
```

## Discussion

The default value of this property is true. Set it to false if you want to disable selecting rows by typing.

