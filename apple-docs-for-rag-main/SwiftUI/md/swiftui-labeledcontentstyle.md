

- SwiftUI
-  LabeledContentStyle 

Protocol

# LabeledContentStyle

The appearance and behavior of a labeled content instance..

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
protocol LabeledContentStyle
```

## Overview

Use labeledContentStyle(_:) to set a style on a view.

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

### Getting built-in labeled content styles

static var automatic: AutomaticLabeledContentStyle

A labeled content style that resolves its appearance automatically based on the current context.

### Creating custom labeled content styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of labeled content.

**Required**

typealias Configuration

The properties of a labeled content instance.

associatedtype Body : View

A view that represents the appearance and behavior of labeled content.

**Required**

### Supporting types

struct AutomaticLabeledContentStyle

The default labeled content style.

## Relationships

### Conforming Types

- AutomaticLabeledContentStyle

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

protocol GroupBoxStyle

A type that specifies the appearance and interaction of all group boxes within a view hierarchy.

struct GroupBoxStyleConfiguration

The properties of a group box instance.

func indexViewStyle&lt;S>(S) -> some View

Sets the style for the index view within the current environment.

protocol IndexViewStyle

Defines the implementation of all `IndexView` instances within a view hierarchy.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

struct LabeledContentStyleConfiguration

The properties of a labeled content instance.

