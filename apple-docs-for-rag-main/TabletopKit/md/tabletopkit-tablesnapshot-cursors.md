

- TabletopKit
- TableSnapshot
-  cursors 

Instance Property

# cursors

visionOS 2.0+

``` source
var cursors: [TableCursor] { get }
```

## See Also

### Getting cursors

func cursor(matching: TableCursorIdentifier) -> TableCursor?

func cursors(forPlayer: Player) -> [TableCursor]

func cursors(hovering: EquipmentIdentifier) -> [TableCursor]

