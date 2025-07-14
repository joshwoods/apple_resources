

- SwiftUI
-  GroupBoxStyle 

Protocol

# GroupBoxStyle

A type that specifies the appearance and interaction of all group boxes within a view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol GroupBoxStyle
```

## Overview

To configure the current `GroupBoxStyle` for a view hierarchy, use the groupBoxStyle(_:) modifier.

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

### Getting built-in group box styles

static var automatic: DefaultGroupBoxStyle

The default style for group box views.

### Creating custom group box styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a group box.

**Required**

typealias Configuration

The properties of a group box instance.

associatedtype Body : View

A view that represents the body of a group box.

**Required**

### Supporting types

struct DefaultGroupBoxStyle

The default style for group box views.

## Relationships

### Conforming Types

- DefaultGroupBoxStyle

## See Also

### Styling groups

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

protocol ControlGroupStyle

Defines the implementation of all control groups within a view hierarchy.

struct ControlGroupStyleConfiguration

The properties of a control group.

func formStyle&lt;S>(S) -> some View

Sets the style for forms in a view hierarchy.

protocol FormStyle

The appearance and behavior of a form.

struct FormStyleConfiguration

The properties of a form instance.

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

struct GroupBoxStyleConfiguration

The properties of a group box instance.

func indexViewStyle&lt;S>(S) -> some View

Sets the style for the index view within the current environment.

protocol IndexViewStyle

Defines the implementation of all `IndexView` instances within a view hierarchy.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

protocol LabeledContentStyle

The appearance and behavior of a labeled content instance..

struct LabeledContentStyleConfiguration

The properties of a labeled content instance.

