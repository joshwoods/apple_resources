

- GameplayKit
- GKRandomSource
-  init() 

Initializer

# init()

Initializes a new random source object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init()
```

## Return Value

An independent random source.

## Discussion

This initializer returns a new random source instance that does not share state with any other randomizer and is suitable for most gameplay uses. Which random source class this initializer creates is may change between OS releases (currently, this initializer returns a GKARC4RandomSource instance). Use this initializer when the choice of randomization algorithm does not matter. If you need a specific randomization algorithm, call the initializer for a specific GKRandomSource subclass.

For more information, see GameplayKit Programming Guide.

