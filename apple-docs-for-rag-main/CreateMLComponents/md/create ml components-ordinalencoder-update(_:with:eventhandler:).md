

- Create ML Components
- OrdinalEncoder
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout OrdinalEncoder.Transformer,
    with input: some Sequence>,
    eventHandler: EventHandler? = nil
) throws
```

Available when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Discussion

Note

You can’t add new categories on subsequent updates. All categories should be present in the initial update.

