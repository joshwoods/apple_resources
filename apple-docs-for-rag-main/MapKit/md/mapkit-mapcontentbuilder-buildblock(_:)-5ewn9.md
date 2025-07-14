

- MapKit
- MapContentBuilder
-  buildBlock(\_:) 

Type Method

# buildBlock(\_:)

Creates a map content block that contains a single content result.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func buildBlock(_ content: C) -> C where C : MapContent
```

## Parameters 

`content`  

The view content to add to the block.

## Return Value

Returns the MapContent with the single element you provided.

## See Also

### Map content builders

static func buildBlock() -> EmptyMapContent

Creates an empty map content block that contains no statements.

