

- Create ML Components
- PoseSelector
-  init(strategy:confidenceThreshold:) 

Initializer

# init(strategy:confidenceThreshold:)

Creates a pose selector.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    strategy: PoseSelectionStrategy,
    confidenceThreshold: Float
)
```

## Parameters 

`strategy`  

The strategy used to choose a pose if multiple poses are detected on the same frame. Default strategy is to select a pose with maximum bounding box area.

`confidenceThreshold`  

A threshold confidence between 0 to 1 for the joints to be considered valid in pose selection. The default value is 0.2.

## See Also

### Creating a selector

init()

Creates a pose selector.

init(strategy: PoseSelectionStrategy)

Creates a pose selector.

