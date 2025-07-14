

- SwiftUI
- CommandGroupPlacement
-  textEditing 

Type Property

# textEditing

Placement for commands that manipulate and transform text selections.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let textEditing: CommandGroupPlacement
```

## Discussion

By default, this group includes the following commands in macOS:

- Find submenu

- Spelling and Grammar submenu

- Substitutions submenu

- Transformations submenu

- Speech submenu

## See Also

### Content updates

static let pasteboard: CommandGroupPlacement

Placement for commands that interact with the Clipboard and manipulate content that is currently selected in the app’s view hierarchy.

static let textFormatting: CommandGroupPlacement

Placement for commands that manipulate and transform the styles applied to text selections.

static let undoRedo: CommandGroupPlacement

Placement for commands that control the Undo Manager.

