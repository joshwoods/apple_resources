

- SwiftUI
- CommandGroupPlacement
-  pasteboard 

Type Property

# pasteboard

Placement for commands that interact with the Clipboard and manipulate content that is currently selected in the app’s view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let pasteboard: CommandGroupPlacement
```

## Discussion

By default, this group includes the following commands in macOS:

- Cut

- Copy

- Paste

- Paste and Match Style

- Delete

- Select All

## See Also

### Content updates

static let textEditing: CommandGroupPlacement

Placement for commands that manipulate and transform text selections.

static let textFormatting: CommandGroupPlacement

Placement for commands that manipulate and transform the styles applied to text selections.

static let undoRedo: CommandGroupPlacement

Placement for commands that control the Undo Manager.

