

- Accessibility
-  AXChart 

Protocol

# AXChart

A protocol that declares the minimum interface necessary for an accessibility element to act as a chart.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AXChart : NSObjectProtocol
```

## Mentioned in 

Representing chart data as an audio graph

## Overview

Use this protocol when you want to create an accessible representation of a chart — a view that displays a graphical representation of a data set — for VoiceOver to play as an audio graph.

Adopt the AXChart protocol on your chart’s view model, and set the accessibilityChartDescriptor property to an AXChartDescriptor that contains all the semantic information you need to represent your chart through an audio interface, like the chart’s title, axes, data points, and a summary of the chart’s key takeaways.

## Topics

### Supporting accessibility

var accessibilityChartDescriptor: AXChartDescriptor?

A semantic description of an accessible chart or graph in the form of a chart descriptor.

**Required**

class AXChartDescriptor

An object that contains all the semantic information about an accessible chart.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Chart representation

class AXChartDescriptor

An object that contains all the semantic information about an accessible chart.

