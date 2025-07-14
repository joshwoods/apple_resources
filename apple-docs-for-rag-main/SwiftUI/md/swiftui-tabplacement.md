

- SwiftUI
-  TabPlacement 

Structure

# TabPlacement

A place that a tab can appear.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TabPlacement
```

## Overview

Not all `TabView` styles support all placements.

## Topics

### Type Properties

static let automatic: TabPlacement

The default tab location.

static let pinned: TabPlacement

The pinned tab placement location.

static let sidebarOnly: TabPlacement

The sidebar tab placement location.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Configuring a tab

func sectionActions&lt;Content>(content: () -> Content) -> some View

Adds custom actions to a section.

struct TabContentBuilder

A result builder that constructs tabs for a tab view that supports programmatic selection. This builder requires that all tabs in the tab view have the same selection type.

protocol TabContent

A type that provides content for programmatically selectable tabs in a tab view.

struct AnyTabContent

Type erased tab content.

