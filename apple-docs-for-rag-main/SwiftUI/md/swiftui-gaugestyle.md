

- SwiftUI
-  GaugeStyle 

Protocol

# GaugeStyle

Defines the implementation of all gauge instances within a view hierarchy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
protocol GaugeStyle
```

## Overview

To configure the style for all the Gauge instances in a view hierarchy, use the gaugeStyle(_:) modifier. For example, you can configure a gauge to use the circular style:

```
Gauge(value: batteryLevel, in: 0...100) {
    Text("Battery Level")
}
.gaugeStyle(.circular)
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

### Getting the automatic style

static var automatic: DefaultGaugeStyle

The default gauge view style in the current context of the view being styled.

### Getting circular gauge styles

static var circular: CircularGaugeStyle

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

static var accessoryCircular: AccessoryCircularGaugeStyle

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

static var accessoryCircularCapacity: AccessoryCircularCapacityGaugeStyle

A gauge style that displays a closed ring that’s partially filled in to indicate the gauge’s current value.

### Getting linear gauge styles

static var linear: LinearGaugeStyle

A gauge style that displays a bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

static var linearCapacity: LinearCapacityGaugeStyle

A gauge style that displays a bar that fills from leading to trailing edges as the gauge’s current value increases.

static var accessoryLinear: AccessoryLinearGaugeStyle

A gauge style that displays bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

static var accessoryLinearCapacity: AccessoryLinearCapacityGaugeStyle

A gauge style that displays bar that fills from leading to trailing edges as the gauge’s current value increases.

### Creating custom gauge styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a gauge.

**Required**

typealias Configuration

The properties of a gauge instance.

associatedtype Body : View

A view representing the body of a gauge.

**Required**

### Supporting types

struct DefaultGaugeStyle

The default gauge view style in the current context of the view being styled.

struct CircularGaugeStyle

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

struct AccessoryCircularGaugeStyle

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

struct AccessoryCircularCapacityGaugeStyle

A gauge style that displays a closed ring that’s partially filled in to indicate the gauge’s current value.

struct LinearGaugeStyle

A gauge style that displays a bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

struct LinearCapacityGaugeStyle

A gauge style that displays bar that fills from leading to trailing edges as the gauge’s current value increases.

struct AccessoryLinearGaugeStyle

A gauge style that displays bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

struct AccessoryLinearCapacityGaugeStyle

A gauge style that displays bar that fills from leading to trailing edges as the gauge’s current value increases.

## Relationships

### Conforming Types

- AccessoryCircularCapacityGaugeStyle
- AccessoryCircularGaugeStyle
- AccessoryLinearCapacityGaugeStyle
- AccessoryLinearGaugeStyle
- CircularGaugeStyle
- DefaultGaugeStyle
- LinearCapacityGaugeStyle
- LinearGaugeStyle

## See Also

### Styling indicators

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

struct GaugeStyleConfiguration

The properties of a gauge instance.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

protocol ProgressViewStyle

A type that applies standard interaction behavior to all progress views within a view hierarchy.

struct ProgressViewStyleConfiguration

The properties of a progress view instance.

