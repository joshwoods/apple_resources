

- SwiftUI
-  DisclosureGroupStyle 

Protocol

# DisclosureGroupStyle

A type that specifies the appearance and interaction of disclosure groups within a view hierarchy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol DisclosureGroupStyle
```

## Overview

To configure the disclosure group style for a view hierarchy, use the disclosureGroupStyle(_:) modifier.

To create a custom disclosure group style, declare a type that conforms to `DisclosureGroupStyle`. Implement the makeBody(configuration:) method to return a view that composes the elements of the `configuration` that SwiftUI provides to your method.

```
struct MyDisclosureStyle: DisclosureGroupStyle {
    func makeBody(configuration: Configuration) -> some View {
        VStack {
            Button {
                withAnimation {
                    configuration.isExpanded.toggle()
                }
            } label: {
                HStack(alignment: .firstTextBaseline) {
                    configuration.label
                    Spacer()
                    Text(configuration.isExpanded ? "hide" : "show")
                        .foregroundColor(.accentColor)
                        .font(.caption.lowercaseSmallCaps())
                        .animation(nil, value: configuration.isExpanded)
                }
                .contentShape(Rectangle())
            }
            .buttonStyle(.plain)
            if configuration.isExpanded {
                configuration.content
            }
        }
    }
}
```

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

### Getting the styles

static var automatic: AutomaticDisclosureGroupStyle

A disclosure group style that resolves its appearance automatically based on the current context.

### Creating custom disclosure group styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a disclosure group.

**Required**

struct DisclosureGroupStyleConfiguration

The properties of a disclosure group instance.

typealias Configuration

The properties of a disclosure group instance.

associatedtype Body : View

A view that represents the body of a disclosure group.

**Required**

### Supporting types

struct AutomaticDisclosureGroupStyle

A disclosure group style that resolves its appearance automatically based on the current context.

## Relationships

### Conforming Types

- AutomaticDisclosureGroupStyle

## See Also

### Styling collection views

func listStyle&lt;S>(S) -> some View

Sets the style for lists within this view.

protocol ListStyle

A protocol that describes the behavior and appearance of a list.

func tableStyle&lt;S>(S) -> some View

Sets the style for tables within this view.

protocol TableStyle

A type that applies a custom appearance to all tables within a view.

struct TableStyleConfiguration

The properties of a table.

func disclosureGroupStyle&lt;S>(S) -> some View

Sets the style for disclosure groups within this view.

