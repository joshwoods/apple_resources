

- AppKit
- NSRuleEditor
-  addRow(\_:) 

Instance Method

# addRow(\_:)

Adds a row to the receiver.

macOS

``` source
@MainActor
func addRow(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that sent the message.

## See Also

### Manipulating Rows

func insertRow(at: Int, with: NSRuleEditor.RowType, asSubrowOfRow: Int, animate: Bool)

Adds a new row of a given type at a given location.

func removeRow(at: Int)

Removes the row at a given index.

func removeRows(at: IndexSet, includeSubrows: Bool)

Removes the rows at given indexes.

