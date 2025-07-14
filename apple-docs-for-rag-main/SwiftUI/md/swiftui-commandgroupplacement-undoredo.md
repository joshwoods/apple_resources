

- SwiftUI
- CommandGroupPlacement
-  undoRedo 

Type Property

# undoRedo

Placement for commands that control the Undo Manager.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let undoRedo: CommandGroupPlacement
```

## Discussion

By default, this group includes the following commands in macOS:

- Undo

- Redo

## See Also

### Content updates

static let pasteboard: CommandGroupPlacement

Placement for commands that interact with the Clipboard and manipulate content that is currently selected in the app’s view hierarchy.

static let textEditing: CommandGroupPlacement

Placement for commands that manipulate and transform text selections.

static let textFormatting: CommandGroupPlacement

Placement for commands that manipulate and transform the styles applied to text selections.

