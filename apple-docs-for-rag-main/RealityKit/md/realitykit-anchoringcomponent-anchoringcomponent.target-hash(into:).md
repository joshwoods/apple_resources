

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the target by feeding them into the given hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hash function to use when combining the components of the target.

## See Also

### Comparing targets

static func == (AnchoringComponent.Target, AnchoringComponent.Target) -> Bool

Indicates whether two targets are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

var hashValue: Int

The hash value.

