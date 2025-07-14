

- SwiftUI
-  LabelStyle 

Protocol

# LabelStyle

A type that applies a custom appearance to all labels within a view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
protocol LabelStyle
```

## Overview

To configure the current label style for a view hierarchy, use the labelStyle(_:) modifier.

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

### Getting built-in label styles

static var automatic: DefaultLabelStyle

A label style that resolves its appearance automatically based on the current context.

static var iconOnly: IconOnlyLabelStyle

A label style that only displays the icon of the label.

static var titleAndIcon: TitleAndIconLabelStyle

A label style that shows both the title and icon of the label using a system-standard layout.

static var titleOnly: TitleOnlyLabelStyle

A label style that only displays the title of the label.

### Creating custom label styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a label.

**Required**

typealias Configuration

The properties of a label.

associatedtype Body : View

A view that represents the body of a label.

**Required**

### Supporting types

struct DefaultLabelStyle

The default label style in the current context.

struct IconOnlyLabelStyle

A label style that only displays the icon of the label.

struct TitleAndIconLabelStyle

A label style that shows both the title and icon of the label using a system-standard layout.

struct TitleOnlyLabelStyle

A label style that only displays the title of the label.

## Relationships

### Conforming Types

- DefaultLabelStyle
- IconOnlyLabelStyle
- TitleAndIconLabelStyle
- TitleOnlyLabelStyle

## See Also

### Styling views that display text

func labelStyle&lt;S>(S) -> some View

Sets the style for labels within this view.

struct LabelStyleConfiguration

The properties of a label.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

protocol TextFieldStyle

A specification for the appearance and interaction of a text field.

func textEditorStyle(some TextEditorStyle) -> some View

Sets the style for text editors within this view.

protocol TextEditorStyle

A specification for the appearance and interaction of a text editor.

struct TextEditorStyleConfiguration

The properties of a text editor.

