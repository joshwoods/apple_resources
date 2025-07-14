

- SwiftUI
- WindowToolbarStyle
-  unified 

Type Property

# unified

A window toolbar style which displays its toolbar and title bar inline.

macOS 11.0+

``` source
static var unified: UnifiedWindowToolbarStyle { get }
```

Available when `Self` is `UnifiedWindowToolbarStyle`.

## See Also

### Getting built-in window toolbar styles

static var automatic: DefaultWindowToolbarStyle

The automatic window toolbar style.

static var expanded: ExpandedWindowToolbarStyle

A window toolbar style which displays its title bar area above the toolbar.

static func unified(showsTitle: Bool) -> UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static var unifiedCompact: UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

static func unifiedCompact(showsTitle: Bool) -> UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

