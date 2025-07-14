

- MapKit
- MapContent
-  tag(\_:) 

Instance Method

# tag(\_:)

Sets the unique tag value of this piece of map content.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func tag(_ tag: V) -> some MapContent where V : Hashable
```

## Parameters 

`tag`  

A Hashable value to use as the map content’s tag.

## Return Value

Map content with the specified tag set.

## Discussion

Use this modifier to differentiate between selectable content in the map. When the map’s selection binding has the same value as the tag applied to a piece of map content, that content is considered selected.

A `ForEach` automatically applies a default tag to each enumerated view using the `id` parameter of the corresponding element. If the element’s `id` parameter and the the map’s selection input have the same type, you can omit the explicit tag modifier.

