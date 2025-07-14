

- Accessibility
-  AXDataAxisDescriptor 

Protocol

# AXDataAxisDescriptor

The basic interface for a data axis in a chart.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AXDataAxisDescriptor : NSCopying
```

## Overview

Each AXChart requires at least two AXDataAxisDescriptor objects to describe an x-axis and a y-axis.

## Topics

### Specifying the title

var title: String

The title of the axis.

**Required**

var attributedTitle: NSAttributedString

An attributed version of the axis title.

**Required**

## Relationships

### Inherits From

- NSCopying

### Conforming Types

- AXCategoricalDataAxisDescriptor
- AXNumericDataAxisDescriptor

## See Also

### Axis representation

class AXCategoricalDataAxisDescriptor

An object that represents an axis of categorical data.

class AXNumericDataAxisDescriptor

An object that represents an axis of numerical data.

