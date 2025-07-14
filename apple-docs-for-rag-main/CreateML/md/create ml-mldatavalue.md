

- Create ML
-  MLDataValue 

Enumeration

# MLDataValue

The value of a cell in a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
enum MLDataValue
```

## Overview

The MLDataValue enumeration is the fundamental type that you use to store training data in a table. Classifiers use data values to store information like evaluation metrics. Data values wrap all of the possible data types you can use with Create ML.

To access the underlying information in a data value, you can use the properties that correspond to the type’s enumeration cases. If you aren’t sure which kind of value a data value wrapper contains, use a switch statement to unwrap the value, or check the value of the type property.

## Topics

### Converting between types and data values

protocol MLDataValueConvertible

A type that can convert itself to and from a data value.

### Creating a data value

case int(Int)

An integer value.

case double(Double)

A double value.

case string(String)

A string value.

case dictionary(MLDataValue.DictionaryType)

A dictionary of named data values.

case sequence(MLDataValue.SequenceType)

A sequence of data values.

case multiArray(MLDataValue.MultiArrayType)

A multidimensional array of data values.

### Inspecting the type

var type: MLDataValue.ValueType

The kind of the underlying value that the data value wraps.

enum ValueType

An enumeration describing the supported underlying types that an `MLDataValue wraps`.

### Accessing numeric values

var intValue: Int?

The underlying integer value.

var doubleValue: Double?

The underlying double value.

### Accessing string values

var stringValue: String?

The underlying string value.

### Accessing dictionary values

var dictionaryValue: MLDataValue.DictionaryType?

The underlying dictionary.

struct DictionaryType

A dictionary of named data values.

### Accessing array values

var sequenceValue: MLDataValue.SequenceType?

The underlying sequence.

struct SequenceType

A sequence of data values.

var multiArrayValue: MLDataValue.MultiArrayType?

The underlying multidimensional array.

struct MultiArrayType

A multidimensional array of data values.

### Comparing data values

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (MLDataValue, MLDataValue) -> Bool

Returns a Boolean value indicating whether two data values wrap the same underlying value.

var hashValue: Int

The hash value.

### Describing a data value

var description: String

A text representation of the data value.

var debugDescription: String

A text representation of the data value that’s suitable for output during debugging.

### Handling errors

case invalid

An invalid value.

var isValid: Bool

A Boolean value indicating whether the data value is valid.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Tabular Data

struct MLDataTable

A table of data for training or evaluating a machine learning model.

Data Visualizations

Render images of data tables and columns in a playground.

