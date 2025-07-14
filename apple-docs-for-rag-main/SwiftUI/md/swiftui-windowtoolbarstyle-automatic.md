

- SwiftUI
- WindowToolbarStyle
-  automatic 

Type Property

# automatic

The automatic window toolbar style.

macOS 11.0+

``` source
static var automatic: DefaultWindowToolbarStyle { get }
```

Available when `Self` is `DefaultWindowToolbarStyle`.

## See Also

### Getting built-in window toolbar styles

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

