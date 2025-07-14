

- RealityKit
- AudioResource
- AudioResource.InputMode
-  ==(\_:\_:) Deprecated

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 13.0–16.3DeprecatediPadOS 13.0–16.3DeprecatedMac Catalyst 13.0–16.3DeprecatedmacOS 10.15–13.3Deprecated

``` source
static func == (a: AudioResource.InputMode, b: AudioResource.InputMode) -> Bool
```

Deprecated

Use the ChannelAudioComponent, AmbientAudioComponent, or SpatialAudioComponent instead.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing input modes

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

Deprecated

var hashValue: Int

The hash value.

Deprecated

