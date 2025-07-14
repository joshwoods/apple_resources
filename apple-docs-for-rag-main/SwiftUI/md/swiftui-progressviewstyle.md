

- SwiftUI
-  ProgressViewStyle 

Protocol

# ProgressViewStyle

A type that applies standard interaction behavior to all progress views within a view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
protocol ProgressViewStyle
```

## Overview

To configure the current progress view style for a view hierarchy, use the progressViewStyle(_:) modifier.

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

### Getting built-in progress view styles

static var automatic: DefaultProgressViewStyle

The default progress view style in the current context of the view being styled.

static var circular: CircularProgressViewStyle

The style of a progress view that uses a circular gauge to indicate the partial completion of an activity.

static var linear: LinearProgressViewStyle

A progress view that visually indicates its progress using a horizontal bar.

### Creating custom progress view styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a progress view.

**Required**

typealias Configuration

A type alias for the properties of a progress view instance.

associatedtype Body : View

A view representing the body of a progress view.

**Required**

### Supporting types

struct DefaultProgressViewStyle

The default progress view style in the current context of the view being styled.

struct CircularProgressViewStyle

A progress view that uses a circular gauge to indicate the partial completion of an activity.

struct LinearProgressViewStyle

A progress view that visually indicates its progress using a horizontal bar.

## Relationships

### Conforming Types

- CircularProgressViewStyle
- DefaultProgressViewStyle
- LinearProgressViewStyle

## See Also

### Styling indicators

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

protocol GaugeStyle

Defines the implementation of all gauge instances within a view hierarchy.

struct GaugeStyleConfiguration

The properties of a gauge instance.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

struct ProgressViewStyleConfiguration

The properties of a progress view instance.

