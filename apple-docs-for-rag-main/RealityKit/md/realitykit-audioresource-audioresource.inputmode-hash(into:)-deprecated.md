

- RealityKit
- AudioResource
- AudioResource.InputMode
-  hash(into:) Deprecated

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

iOS 13.0–16.3DeprecatediPadOS 13.0–16.3DeprecatedMac Catalyst 13.0–16.3DeprecatedmacOS 10.15–13.3Deprecated

``` source
func hash(into hasher: inout Hasher)
```

Deprecated

Use the ChannelAudioComponent, AmbientAudioComponent, or SpatialAudioComponent instead.

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## Discussion

Implement this method to conform to the `Hashable` protocol. The components used for hashing must be the same as the components compared in your type’s `==` operator implementation. Call `hasher.combine(_:)` with each of these components.

Important

In your implementation of `hash(into:)`, don’t call `finalize()` on the `hasher` instance provided, or replace it with a different instance. Doing so may become a compile-time error in the future.

## See Also

### Comparing input modes

static func == (AudioResource.InputMode, AudioResource.InputMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

Deprecated

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

var hashValue: Int

The hash value.

Deprecated

