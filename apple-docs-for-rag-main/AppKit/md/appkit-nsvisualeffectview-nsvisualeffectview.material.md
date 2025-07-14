

- AppKit
- NSVisualEffectView
-  NSVisualEffectView.Material 

Enumeration

# NSVisualEffectView.Material

Constants to specify the material shown by the visual effect view.

macOS 10.10+

``` source
enum Material
```

## Topics

### Material Types

case titlebar

The material for a window’s titlebar.

case selection

The material used to indicate a selection.

case menu

The material for menus.

case popover

The material for the background of popover windows.

case sidebar

The material for the background of window sidebars.

case headerView

The material for in-line header or footer views.

case sheet

The material for the background of sheet windows.

case windowBackground

The material for the background of opaque windows.

case hudWindow

The material for the background of heads-up display (HUD) windows.

case fullScreenUI

The material for the background of a full-screen modal interface.

case toolTip

The material for the background of a tool tip.

case contentBackground

The material for the background of opaque content.

case underWindowBackground

The material to show under a window’s background.

case underPageBackground

The material for the area behind the pages of a document.

### Deprecated Materials

case appearanceBased

A default material for the view’s effective appearance.

Deprecated

case light

A material with a light effect.

Deprecated

case dark

A material with a dark effect.

Deprecated

case mediumLight

A material with a medium-light effect.

Deprecated

case ultraDark

A material with an ultra-dark effect.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the Background Material

var material: NSVisualEffectView.Material

The material shown by the visual effect view.

