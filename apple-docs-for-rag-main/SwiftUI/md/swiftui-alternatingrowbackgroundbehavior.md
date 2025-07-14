

- SwiftUI
-  AlternatingRowBackgroundBehavior 

Structure

# AlternatingRowBackgroundBehavior

The styling of views with respect to alternating row backgrounds.

macOS 14.0+

``` source
struct AlternatingRowBackgroundBehavior
```

## Overview

Use values of this type with the alternatingRowBackgrounds(_:) modifier.

## Topics

### Getting alternating row background behavior

static let automatic: AlternatingRowBackgroundBehavior

The automatic alternating row background behavior.

static let enabled: AlternatingRowBackgroundBehavior

Alternating rows will be enabled for applicable views.

static let disabled: AlternatingRowBackgroundBehavior

Alternating rows will be disabled for applicable views.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring backgrounds

func listRowBackground&lt;V>(V?) -> some View

Places a custom background view behind a list row item.

func alternatingRowBackgrounds(AlternatingRowBackgroundBehavior) -> some View

Overrides whether lists and tables in this view have alternating row backgrounds.

var backgroundProminence: BackgroundProminence

The prominence of the background underneath views associated with this environment.

struct BackgroundProminence

The prominence of backgrounds underneath other views.

