

- SwiftUI
- EnvironmentValues
-  badgeProminence 

Instance Property

# badgeProminence

The prominence to apply to badges associated with this environment.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var badgeProminence: BadgeProminence { get set }
```

## Discussion

The default is standard.

## See Also

### Displaying a badge on a list item

func badge(_:)

Generates a badge for the view from an integer value.

func badgeProminence(BadgeProminence) -> some View

Specifies the prominence of badges created by this view.

struct BadgeProminence

The visual prominence of a badge.

