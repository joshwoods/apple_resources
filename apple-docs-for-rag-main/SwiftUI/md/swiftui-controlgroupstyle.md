

- SwiftUI
-  ControlGroupStyle 

Protocol

# ControlGroupStyle

Defines the implementation of all control groups within a view hierarchy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol ControlGroupStyle
```

## Overview

To configure the current `ControlGroupStyle` for a view hierarchy, use the controlGroupStyle(_:) modifier.

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

### Getting built-in control group styles

static var automatic: AutomaticControlGroupStyle

The default control group style.

static var compactMenu: CompactMenuControlGroupStyle

A control group style that presents its content as a compact menu when the user presses the control, or as a submenu when nested within a larger menu.

static var menu: MenuControlGroupStyle

A control group style that presents its content as a menu when the user presses the control, or as a submenu when nested within a larger menu.

static var navigation: NavigationControlGroupStyle

The navigation control group style.

static var palette: PaletteControlGroupStyle

A control group style that presents its content as a palette.

### Creating custom control group styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a control group.

**Required**

typealias Configuration

The properties of a `ControlGroup` instance being created.

associatedtype Body : View

A view representing the body of a control group.

**Required**

### Supporting types

struct AutomaticControlGroupStyle

The default control group style.

struct CompactMenuControlGroupStyle

A control group style that presents its content as a compact menu when the user presses the control, or as a submenu when nested within a larger menu.

struct MenuControlGroupStyle

A control group style that presents its content as a menu when the user presses the control, or as a submenu when nested within a larger menu.

struct NavigationControlGroupStyle

The navigation control group style.

struct PaletteControlGroupStyle

A control group style that presents its content as a palette.

## Relationships

### Conforming Types

- AutomaticControlGroupStyle
- CompactMenuControlGroupStyle
- MenuControlGroupStyle
- NavigationControlGroupStyle
- PaletteControlGroupStyle

## See Also

### Styling groups

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

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

protocol LabeledContentStyle

The appearance and behavior of a labeled content instance..

struct LabeledContentStyleConfiguration

The properties of a labeled content instance.

