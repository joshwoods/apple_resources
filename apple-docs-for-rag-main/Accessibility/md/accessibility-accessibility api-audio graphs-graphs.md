

- Accessibility
- Accessibility API
-  Audio graphs 

API Collection

# Audio graphs

Define an accessible representation of your chart for VoiceOver to generate an audio graph.

## Overview

Charts and graphs help users quickly identify important features and trends in data. Use the audio graphs API to provide all the information that VoiceOver needs to construct an audible representation of the data in your charts and graphs, making the data accessible to people who are blind or have low vision.

An *audio graph* turns the data in your chart into an audible representation by encoding the data on each axis as audio. Typically, the audio graph represents the x-axis as time, and the y-axis as pitch. For example, an audible representation of a scatter plot that shows a linear downward trend might be a series of individual tones descending in pitch over time. An audible representation of a stock chart might be a single continuous tone with a pitch that modulates up or down with the stock price (y-axis) as the audio plays over time (x-axis).

Related sessions from WWDC21

Session 10122: Bring accessibility to charts in your app

## Topics

### Essentials

Representing chart data as an audio graph

Define accessible representations of your chart’s components for VoiceOver to construct an audible representation of the data.

### Chart representation

protocol AXChart

A protocol that declares the minimum interface necessary for an accessibility element to act as a chart.

class AXChartDescriptor

An object that contains all the semantic information about an accessible chart.

### Axis representation

protocol AXDataAxisDescriptor

The basic interface for a data axis in a chart.

class AXCategoricalDataAxisDescriptor

An object that represents an axis of categorical data.

class AXNumericDataAxisDescriptor

An object that represents an axis of numerical data.

### Data representation

class AXDataPoint

An object that represents a single data point in a chart.

class AXDataSeriesDescriptor

An object that represents a series of data points.

### Live audio graphs

class AXLiveAudioGraph

An object that represents an audio graph for a live-updating, continuous data series for VoiceOver.

## See Also

### Features

Customized accessibility content

Customize your apps to deliver accessibility information to your users in measured portions as they need it.

Braille displays

Display a graphical representation of images, icons, data, and more on a two-dimensional braille display.

Hearing device support

Access information about paired hearing aid devices and streaming status.

func AXNameFromColor(CGColor) -> String

Returns a localized description of the color to use in accessibility attributes.

