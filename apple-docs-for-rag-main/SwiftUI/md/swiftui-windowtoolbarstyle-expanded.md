

- SwiftUI
- WindowToolbarStyle
-  expanded 

Type Property

# expanded

A window toolbar style which displays its title bar area above the toolbar.

macOS 11.0+

``` source
static var expanded: ExpandedWindowToolbarStyle { get }
```

Available when `Self` is `ExpandedWindowToolbarStyle`.

## See Also

### Getting built-in window toolbar styles

static var automatic: DefaultWindowToolbarStyle

The automatic window toolbar style.

static var unified: UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static func unified(showsTitle: Bool) -> UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static var unifiedCompact: UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

static func unifiedCompact(showsTitle: Bool) -> UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

