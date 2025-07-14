

- RealityKit
- AnimationPlaybackController
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two animation playback controllers are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func == (lhs: AnimationPlaybackController, rhs: AnimationPlaybackController) -> Bool
```

## Parameters 

`lhs`  

The first controller to compare.

`rhs`  

The second controller to compare.

## Return Value

A Boolean value set to `true` if the two controllers are equal.

## See Also

### Comparing animation playback controllers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the controller by feeding them into the given hash function.

var hashValue: Int

The hash value.

