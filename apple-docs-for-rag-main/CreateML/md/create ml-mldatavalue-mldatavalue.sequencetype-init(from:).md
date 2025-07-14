

- Create ML
- MLDataValue
- MLDataValue.SequenceType
-  init(from:) 

Initializer

# init(from:)

Creates a data-value sequence from another sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init?(from dataValue: MLDataValue)
```

## Discussion

Use this initializer to create an MLDataValue.SequenceType from another data-value sequence instance. You can confirm the data value’s underlying type by retrieving a non-`nil` value from sequenceValue or by inspecting the type property.

