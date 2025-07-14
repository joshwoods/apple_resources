

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two targets are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
static func == (lhs: AnchoringComponent.Target, rhs: AnchoringComponent.Target) -> Bool
```

## Parameters 

`lhs`  

The first target to compare.

`rhs`  

The second target to compare.

## Return Value

A Boolean value set to `true` if the two targets are equal.

## See Also

### Comparing targets

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the target by feeding them into the given hash function.

var hashValue: Int

The hash value.

