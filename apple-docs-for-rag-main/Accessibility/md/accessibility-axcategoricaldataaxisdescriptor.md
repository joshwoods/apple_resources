

- Accessibility
-  AXCategoricalDataAxisDescriptor 

Class

# AXCategoricalDataAxisDescriptor

An object that represents an axis of categorical data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXCategoricalDataAxisDescriptor
```

## Overview

A categorical data axis divides information into groups, or categories. For example, a categorical axis may represent blood type data divided into the possible categories *AB*, *A*, *B*, and *O*.

## Topics

### Creating a categorial data axis

init(title: String, categoryOrder: [String])

Creates a categorical data axis with the specified title and an array of categories in the specified order.

init(attributedTitle: NSAttributedString, categoryOrder: [String])

Creates a categorical data axis with the specified attributed title and an array of categories in the specified order.

### Configuring the order of categories

var categoryOrder: [String]

A list of every category value for the axis in the order they appear visually in the graph or legend.

## Relationships

### Inherits From

- NSObject

### Conforms To

- AXDataAxisDescriptor
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Axis representation

protocol AXDataAxisDescriptor

The basic interface for a data axis in a chart.

class AXNumericDataAxisDescriptor

An object that represents an axis of numerical data.

