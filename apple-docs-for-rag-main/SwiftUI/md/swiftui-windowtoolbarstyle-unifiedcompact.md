

- SwiftUI
- WindowToolbarStyle
-  unifiedCompact 

Type Property

# unifiedCompact

A window toolbar style similar to unified, but with a more compact vertical sizing.

macOS 11.0+

``` source
static var unifiedCompact: UnifiedCompactWindowToolbarStyle { get }
```

Available when `Self` is `UnifiedCompactWindowToolbarStyle`.

## See Also

### Getting built-in window toolbar styles

static var automatic: DefaultWindowToolbarStyle

The automatic window toolbar style.

static var expanded: ExpandedWindowToolbarStyle

A window toolbar style which displays its title bar area above the toolbar.

static var unified: UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static func unified(showsTitle: Bool) -> UnifiedWindowToolbarStyle

A window toolbar style which displays its toolbar and title bar inline.

static func unifiedCompact(showsTitle: Bool) -> UnifiedCompactWindowToolbarStyle

A window toolbar style similar to unified, but with a more compact vertical sizing.

