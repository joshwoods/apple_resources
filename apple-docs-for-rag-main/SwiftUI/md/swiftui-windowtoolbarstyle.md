

- SwiftUI
-  WindowToolbarStyle 

Protocol

# WindowToolbarStyle

A specification for the appearance and behavior of a window’s toolbar.

macOS 11.0+

``` source
protocol WindowToolbarStyle
```

## Topics

### Getting built-in window toolbar styles

static var automatic: DefaultWindowToolbarStyle

The automatic window toolbar style.

static var expanded: ExpandedWindowToolbarStyle

A window toolbar style which displays its title bar area above the toolbar.

static var unified: UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static func unified(showsTitle: Bool) -> UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static var unifiedCompact: UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

static func unifiedCompact(showsTitle: Bool) -> UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

### Supporting types

struct DefaultWindowToolbarStyle

The default window toolbar style.

struct ExpandedWindowToolbarStyle

A window toolbar style which displays its title bar area above the toolbar.

struct UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

struct UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

## Relationships

### Conforming Types

- DefaultWindowToolbarStyle
- ExpandedWindowToolbarStyle
- UnifiedCompactWindowToolbarStyle
- UnifiedWindowToolbarStyle

## See Also

### Styling a toolbar

func toolbarBackground(_:for:)

Specifies the preferred shape style of the background of a bar managed by SwiftUI.

func toolbarColorScheme(ColorScheme?, for: ToolbarPlacement...) -> some View

Specifies the preferred color scheme of a bar managed by SwiftUI.

func toolbarForegroundStyle&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred foreground style of bars managed by SwiftUI.

func windowToolbarStyle&lt;S>(S) -> some Scene

Sets the style for the toolbar defined within this scene.

var toolbarLabelStyle: ToolbarLabelStyle?

The label style to apply to controls within a toolbar.

struct ToolbarLabelStyle

The label style of a toolbar.

