

- SwiftUI
-  TabContentBuilder 

Structure

# TabContentBuilder

A result builder that constructs tabs for a tab view that supports programmatic selection. This builder requires that all tabs in the tab view have the same selection type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@resultBuilder
struct TabContentBuilder where TabValue : Hashable
```

## Topics

### Structures

struct Content

A view representation of the content of a builder-based tab view with selection.

### Type Methods

static func buildBlock(some TabContent&lt;TabValue>) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1>(C0, C1) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2>(C0, C1, C2) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3>(C0, C1, C2, C3) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3, C4>(C0, C1, C2, C3, C4) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3, C4, C5>(C0, C1, C2, C3, C4, C5) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6>(C0, C1, C2, C3, C4, C5, C6) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7>(C0, C1, C2, C3, C4, C5, C6, C7) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> some TabContent&lt;TabValue> 

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> some TabContent&lt;TabValue> 

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

static func buildExpression(some TabContent&lt;TabValue>) -> some TabContent&lt;TabValue> 

static func buildIf((some TabContent&lt;TabValue>)?) -> (some TabContent&lt;TabValue>)? 

static func buildLimitedAvailability&lt;T>(T) -> AnyTabContent&lt;T.TabValue>

## See Also

### Configuring a tab

func sectionActions&lt;Content>(content: () -> Content) -> some View

Adds custom actions to a section.

struct TabPlacement

A place that a tab can appear.

protocol TabContent

A type that provides content for programmatically selectable tabs in a tab view.

struct AnyTabContent

Type erased tab content.

