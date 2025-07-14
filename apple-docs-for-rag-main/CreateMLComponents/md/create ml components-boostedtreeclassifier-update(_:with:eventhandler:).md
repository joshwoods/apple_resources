

- Create ML Components
- BoostedTreeClassifier
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout TreeClassifierModel,
    with input: DataFrame,
    eventHandler: EventHandler?
) async throws
```

Available when `Label` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A data frame containing examples.

`eventHandler`  

An event handler.

