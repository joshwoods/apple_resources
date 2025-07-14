

- Create ML
- MLDataValue
- MLDataValue.DictionaryType
-  init(from:) 

Initializer

# init(from:)

Creates a data-value dictionary from another dictionary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init?(from dataValue: MLDataValue)
```

## Discussion

Use this initializer to create an MLDataValue.DictionaryType from another data-value dictionary instance. You can confirm the data value’s underlying type by retrieving a non-`nil` value from dictionaryValue or by inspecting the type property.

