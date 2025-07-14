

- SwiftUI
-  BadgeProminence 

Structure

# BadgeProminence

The visual prominence of a badge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct BadgeProminence
```

## Overview

Badges can be used for different kinds of information, from the passive number of items in a container to the number of required actions. The prominence of badges in Lists can be adjusted to reflect this and be made to draw more or less attention to themselves.

Badges will default to `standard` prominence unless specified.

The following example shows a List displaying a list of folders with an informational badge with lower prominence, showing the number of items in the folder.

```
List(folders) { folder in
    Text(folder.name)
        .badge(folder.numberOfItems)
}
.badgeProminence(.decreased)
```

## Topics

### Getting background prominence

static let standard: BadgeProminence

The standard level of prominence for a badge.

static let increased: BadgeProminence

The highest level of prominence for a badge.

static let decreased: BadgeProminence

The lowest level of prominence for a badge.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Displaying a badge on a list item

func badge(_:)

Generates a badge for the view from an integer value.

func badgeProminence(BadgeProminence) -> some View

Specifies the prominence of badges created by this view.

var badgeProminence: BadgeProminence

The prominence to apply to badges associated with this environment.

