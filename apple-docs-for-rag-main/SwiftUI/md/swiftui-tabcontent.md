

- SwiftUI
-  TabContent 

Protocol

# TabContent

A type that provides content for programmatically selectable tabs in a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
protocol TabContent
```

## Overview

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Associated Types

associatedtype Body : TabContent

The type of content representing the body of this content type.

**Required**

associatedtype TabValue : Hashable

The type used to drive selection for the containing tab view.

**Required**

### Instance Properties

var body: Self.Body

The value of this type’s nested content.

**Required**

### Instance Methods

func accessibilityHint(_:isEnabled:)

Communicates to the user what happens after selecting the tab.

func accessibilityIdentifier(String, isEnabled: Bool) -> some TabContent&lt;Self.TabValue> 

Uses the string you specify to identify the view. Use this value for testing. It isn’t visible to the user.

func accessibilityInputLabels(_:isEnabled:)

Sets alternate input labels with which users identify a tab.

func accessibilityLabel(_:isEnabled:)

Adds a label to the tab that describes its contents.

func accessibilityValue(_:isEnabled:)

Adds a textual description of the value that the tab contains.

func badge(_:)

Generates a badge for a tab from an integer value.

func contextMenu&lt;M>(menuItems: () -> M) -> some TabContent&lt;Self.TabValue> 

Adds a context menu to a tab.

func customizationBehavior(TabCustomizationBehavior, for: AdaptableTabBarPlacement...) -> some TabContent&lt;Self.TabValue> 

Configures the customization behavior of customizable tab view content.

func customizationID(String) -> some TabContent&lt;Self.TabValue> 

Sets the identifier for a tab to persist its state.

func defaultVisibility(Visibility, for: AdaptableTabBarPlacement...) -> some TabContent&lt;Self.TabValue> 

Configures the default visibility of a tab in customizable contexts.

func disabled(Bool) -> some TabContent&lt;Self.TabValue> 

Controls whether users can interact with this tab.

func draggable&lt;T>(@autoclosure () -> T) -> some TabContent&lt;Self.TabValue> 

Activates this tab as the source of a drag and drop operation. This tab can only be dragged when in the sidebar.

func dropDestination&lt;T>(for: T.Type, action: ([T]) -> Void) -> some TabContent&lt;Self.TabValue> 

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func hidden(Bool) -> some TabContent&lt;Self.TabValue> 

Hides the tab from the user.

func popover&lt;Content>(isPresented: Binding&lt;Bool>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: () -> Content) -> some TabContent&lt;Self.TabValue> 

Presents a popover when a given condition is true.

func popover&lt;Item, Content>(item: Binding&lt;Item?>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: (Item) -> Content) -> some TabContent&lt;Self.TabValue> 

Presents a popover using the given item as a data source for the popover’s content.

func sectionActions&lt;Content>(content: () -> Content) -> some TabContent&lt;Self.TabValue> 

Adds custom actions to a tab section.

func springLoadingBehavior(SpringLoadingBehavior) -> some TabContent&lt;Self.TabValue> 

Sets the spring loading behavior for the tab.

func swipeActions&lt;T>(edge: HorizontalEdge, allowsFullSwipe: Bool, content: () -> T) -> some TabContent&lt;Self.TabValue> 

Adds custom swipe actions to a tab in a tab view.

func tabPlacement(TabPlacement) -> some TabContent&lt;Self.TabValue> 

Specifies the placement of a tab.

## Relationships

### Conforming Types

- AnyTabContent
- ForEach

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TabContent`.

- Group

  Conforms when `Content` conforms to `TabContent`.

- Tab

  Conforms when `Value` conforms to `Hashable`, `Content` conforms to `View`, and `Label` conforms to `View`.

- TabSection

  Conforms when `Header` conforms to `View`, `Content` conforms to `TabContent`, `Footer` conforms to `View`, and `SelectionValue` is `Content.TabValue`.

## See Also

### Configuring a tab

func sectionActions&lt;Content>(content: () -> Content) -> some View

Adds custom actions to a section.

struct TabPlacement

A place that a tab can appear.

struct TabContentBuilder

A result builder that constructs tabs for a tab view that supports programmatic selection. This builder requires that all tabs in the tab view have the same selection type.

struct AnyTabContent

Type erased tab content.

