

- RealityKit
- AudioResource
- AudioResource.InputMode
-  hashValue Deprecated

Instance Property

# hashValue

The hash value.

iOS 13.0–16.3DeprecatediPadOS 13.0–16.3DeprecatedMac Catalyst 13.0–16.3DeprecatedmacOS 10.15–13.3Deprecated

``` source
var hashValue: Int { get }
```

Deprecated

Use the ChannelAudioComponent, AmbientAudioComponent, or SpatialAudioComponent instead.

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Comparing input modes

static func == (AudioResource.InputMode, AudioResource.InputMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

Deprecated

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

Deprecated

