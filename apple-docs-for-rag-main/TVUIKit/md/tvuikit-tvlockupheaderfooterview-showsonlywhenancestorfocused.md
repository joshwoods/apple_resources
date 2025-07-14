

- TVUIKit
- TVLockupHeaderFooterView
-  showsOnlyWhenAncestorFocused 

Instance Property

# showsOnlyWhenAncestorFocused

A Boolean value indicating whether titles and subtitles are displayed when a lockup view isn’t in focus.

tvOS 12.0+

``` source
@MainActor
var showsOnlyWhenAncestorFocused: Bool { get set }
```

## Discussion

Set this value to `FALSE` to display header and footer information while the lockup view is not in focus. Header and footer information is always shown when a lockup view is in focus, regardless of this property’s value.

