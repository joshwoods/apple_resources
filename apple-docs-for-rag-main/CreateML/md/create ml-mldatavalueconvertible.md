

- Create ML
-  MLDataValueConvertible 

Protocol

# MLDataValueConvertible

A type that can convert itself to and from a data value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
protocol MLDataValueConvertible
```

## Overview

You can use any type that conforms to the MLDataValueConvertible protocol in an MLDataValue or an MLDataTable. For example, you can create a data table by using its init(dictionary:) initializer with a `[`String``` : ``MLDataValueConvertible``] ``` dictionary.

## Topics

### Converting from a data value to a type’s instance

init()

Creates a new default instance of the conforming type when a data value is missing or invalid.

**Required**

init?(from: MLDataValue)

Creates an instance of the conforming type from a data value.

**Required**

### Converting from a type’s instance to a data value

var dataValue: MLDataValue

The value of the conforming type’s instance wrapped in a data value.

**Required**

static var dataValueType: MLDataValue.ValueType

The underlying type the conforming type uses when it wraps itself in a data value.

**Required**

## Relationships

### Conforming Types

- MLDataValue.DictionaryType
- MLDataValue.MultiArrayType
- MLDataValue.SequenceType

