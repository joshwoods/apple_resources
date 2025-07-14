

- ClassKit
- CLSBinaryItem
-  init(identifier:title:type:) 

Initializer

# init(identifier:title:type:)

Initializes a new binary activity item of the given type.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
init(
    identifier: String,
    title: String,
    type valueType: CLSBinaryValueType
)
```

## Parameters 

`identifier`  

A unique identifier for the activity item.

`title`  

A human readable name for the activity item.

`valueType`  

The kind of Boolean that the activity item represents.

## See Also

### Creating Binary Activity Items

enum CLSBinaryValueType

The kinds of outcomes that a binary activity item can represent.

