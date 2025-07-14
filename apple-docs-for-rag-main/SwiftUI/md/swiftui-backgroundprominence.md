

- SwiftUI
-  BackgroundProminence 

Structure

# BackgroundProminence

The prominence of backgrounds underneath other views.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct BackgroundProminence
```

## Overview

Background prominence should influence foreground styling to maintain sufficient contrast against the background. For example, selected rows in a `List` and `Table` can have increased prominence backgrounds with accent color fills when focused; the foreground content above the background should be adjusted to reflect that level of prominence.

This can be read and written for views with the `EnvironmentValues.backgroundProminence` property.

## Topics

### Getting background prominence

static let standard: BackgroundProminence

The standard prominence of a background

static let increased: BackgroundProminence

A more prominent background that likely requires some changes to the views above it.

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

struct AlternatingRowBackgroundBehavior

The styling of views with respect to alternating row backgrounds.

var backgroundProminence: BackgroundProminence

The prominence of the background underneath views associated with this environment.

