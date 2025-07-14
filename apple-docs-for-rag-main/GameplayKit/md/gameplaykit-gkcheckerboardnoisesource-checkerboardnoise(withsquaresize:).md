

- GameplayKit
- GKCheckerboardNoiseSource
-  checkerboardNoise(withSquareSize:) 

Type Method

# checkerboardNoise(withSquareSize:)

Creates a checkerboard noise source with the specified square size.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class func checkerboardNoise(withSquareSize squareSize: Double) -> Self
```

## Parameters 

`squareSize`  

The initial value for the squareSize property, which determines the size of the checkerboard pattern.

## Return Value

A new noise source.

## Discussion

To make use of this noise source, create a GKNoise object from it (and optionally apply operations to that noise object or combine it with other noise objects). Then create a GKNoiseMap object from your noise object, generating a concrete field of values that you can sample from directly or visualize using the SKTexture or `SKTileMap` class.

## See Also

### Creating a Noise Source

init(squareSize: Double)

Initializes a checkerboard noise source with the specified square size.

