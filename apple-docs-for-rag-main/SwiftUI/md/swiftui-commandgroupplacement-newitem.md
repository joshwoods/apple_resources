

- SwiftUI
- CommandGroupPlacement
-  newItem 

Type Property

# newItem

Placement for commands that create and open different kinds of documents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let newItem: CommandGroupPlacement
```

## Discussion

By default, this group includes the following commands in macOS:

- New

- Open

- Open Recent submenu (managed automatically)

## See Also

### File manipulation

static let importExport: CommandGroupPlacement

Placement for commands that relate to importing and exporting data using formats that the app doesn’t natively support.

static let printItem: CommandGroupPlacement

Placement for commands related to printing app content.

static let saveItem: CommandGroupPlacement

Placement for commands that save open documents and close windows.

