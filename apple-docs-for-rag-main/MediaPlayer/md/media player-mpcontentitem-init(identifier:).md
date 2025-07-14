

- Media Player
- MPContentItem
-  init(identifier:) 

Initializer

# init(identifier:)

Sets the identifier for a media item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

A unique identifier for the content item.

## Return Value

The created `MPContentItem` object.

## Discussion

Each media item identifier must be unique. The use of nonunique identifiers can prevent media items from updating properly. Create a new identifier when creating an `MPContentItem` object.

