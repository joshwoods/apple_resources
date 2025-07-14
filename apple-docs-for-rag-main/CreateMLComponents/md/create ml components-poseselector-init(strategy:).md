

- Create ML Components
- PoseSelector
-  init(strategy:) 

Initializer

# init(strategy:)

Creates a pose selector.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(strategy: PoseSelectionStrategy)
```

## Parameters 

`strategy`  

The strategy used to choose a pose if multiple poses are detected on the same frame. Default strategy is to select a pose with maximum bounding box area.

## See Also

### Creating a selector

init()

Creates a pose selector.

init(strategy: PoseSelectionStrategy, confidenceThreshold: Float)

Creates a pose selector.

