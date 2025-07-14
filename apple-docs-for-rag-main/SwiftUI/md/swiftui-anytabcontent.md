

- SwiftUI
-  AnyTabContent 

Structure

# AnyTabContent

Type erased tab content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AnyTabContent where SelectionValue : Hashable
```

## Topics

### Initializers

init&lt;T>(T)

Create an instance that type-erases `tabContent`.

## Relationships

### Conforms To

- TabContent

## See Also

### Configuring a tab

func sectionActions&lt;Content>(content: () -> Content) -> some View

Adds custom actions to a section.

struct TabPlacement

A place that a tab can appear.

struct TabContentBuilder

A result builder that constructs tabs for a tab view that supports programmatic selection. This builder requires that all tabs in the tab view have the same selection type.

protocol TabContent

A type that provides content for programmatically selectable tabs in a tab view.

